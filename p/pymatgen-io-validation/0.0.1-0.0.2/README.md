# Comparing `tmp/pymatgen-io-validation-0.0.1.tar.gz` & `tmp/pymatgen_io_validation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-io-validation-0.0.1.tar", last modified: Tue Mar 19 23:55:09 2024, max compression
+gzip compressed data, was "pymatgen_io_validation-0.0.2.tar", last modified: Fri May  3 19:07:40 2024, max compression
```

## Comparing `pymatgen-io-validation-0.0.1.tar` & `pymatgen_io_validation-0.0.2.tar`

### file list

```diff
@@ -1,138 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.998170 pymatgen-io-validation-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.982170 pymatgen-io-validation-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.982170 pymatgen-io-validation-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/.github/workflows/release_bak.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-03-19 23:55:08.998170 pymatgen-io-validation-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.982170 pymatgen-io-validation-0.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.986170 pymatgen-io-validation-0.0.1/examples/MP_compliant/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/CONTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)    19720 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/DOSCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/EIGENVAL.gz
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/IBZKPT.gz
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/INCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/INCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/MP_compatible_GaAs_r2SCAN_static.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/OSZICAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)    30456 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/OUTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/PCDAT.gz
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/POSCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/POSCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/POTCAR.spec.gz
--rw-r--r--   0 runner    (1001) docker     (127)    52549 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/PROCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/REPORT.gz
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/XDATCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/custodian.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/vasp.out.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72392 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant/vasprun.xml.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_compliant_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.986170 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/CONTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)    19588 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/DOSCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/EIGENVAL.gz
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/IBZKPT.gz
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/INCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/INCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/MP_incompatible_GaAs_r2SCAN_static.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/OSZICAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)    24618 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/OUTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/PCDAT.gz
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/POSCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/POSCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/POTCAR.spec.gz
--rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/PROCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/REPORT.gz
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/XDATCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/custodian.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/vasp.out.gz
--rw-r--r--   0 runner    (1001) docker     (127)    34419 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/MP_non_compliant/vasprun.xml.gz
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/examples/using_validation_docs.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.978170 pymatgen-io-validation-0.0.1/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.978170 pymatgen-io-validation-0.0.1/pymatgen/io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.990170 pymatgen-io-validation-0.0.1/pymatgen/io/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_common_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_for_excess_empty_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    42273 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_incar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_kpoints_kspacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_potcar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/compare_to_MP_ehull.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pymatgen/io/validation/vasp_defaults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.990170 pymatgen-io-validation-0.0.1/pymatgen_io_validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-03-19 23:55:08.000000 pymatgen-io-validation-0.0.1/pymatgen_io_validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-03-19 23:55:08.000000 pymatgen-io-validation-0.0.1/pymatgen_io_validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 23:55:08.000000 pymatgen-io-validation-0.0.1/pymatgen_io_validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 23:55:08.000000 pymatgen-io-validation-0.0.1/pymatgen_io_validation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 23:55:08.000000 pymatgen-io-validation-0.0.1/pymatgen_io_validation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-19 23:55:08.998170 pymatgen-io-validation-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.990170 pymatgen-io-validation-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.978170 pymatgen-io-validation-0.0.1/tests/test_files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.990170 pymatgen-io-validation-0.0.1/tests/test_files/vasp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.994170 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/CONTCAR.relax1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/CONTCAR.relax2.gz
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/IBZKPT.relax1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/IBZKPT.relax2.gz
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/INCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/INCAR.relax1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/INCAR.relax2.gz
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/KPOINTS.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/KPOINTS.relax1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/KPOINTS.relax2.gz
--rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/OUTCAR.relax1.gz
--rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/OUTCAR.relax2.gz
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/POSCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/POSCAR.relax1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/POSCAR.relax2.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/custodian.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/vasp.out.relax1.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/vasp.out.relax2.gz
--rw-r--r--   0 runner    (1001) docker     (127)    35483 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/vasprun.xml.relax1.gz
--rw-r--r--   0 runner    (1001) docker     (127)    33968 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_old_double_relax/vasprun.xml.relax2.gz
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_potcar_spec.json.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.994170 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_static/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_static/CONTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_static/INCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_static/INCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)    19976 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_static/OUTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_static/POSCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_static/POSCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_static/custodian.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)    51310 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_static/vasprun.xml.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.994170 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/CONTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/INCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/INCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/KPOINTS.gz
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/KPOINTS.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/OUTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/POSCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/POSCAR.orig.gz
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/custodian.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)   159022 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/Si_uniform/vasprun.xml.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.994170 pymatgen-io-validation-0.0.1/tests/test_files/vasp/TaskDocuments/
--rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/TaskDocuments/MP_compatible_GaAs_r2SCAN_static_TaskDocument.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)    20899 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/TaskDocuments/MP_incompatible_GaAs_r2SCAN_static_TaskDocument.json.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 23:55:08.994170 pymatgen-io-validation-0.0.1/tests/test_files/vasp/magnetic_run/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/magnetic_run/CONTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)    31482 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/magnetic_run/OUTCAR.gz
--rw-r--r--   0 runner    (1001) docker     (127)   682453 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/magnetic_run/vasprun.xml.gz
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/scf_incar_check_list.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    32640 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_files/vasp/test_GGA_NSCF_calc.json
--rw-r--r--   0 runner    (1001) docker     (127)    25165 2024-03-19 23:55:00.000000 pymatgen-io-validation-0.0.1/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.836586 pymatgen_io_validation-0.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/examples/MP_compliant_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.832586 pymatgen_io_validation-0.0.2/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.832586 pymatgen_io_validation-0.0.2/pymatgen/io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.836586 pymatgen_io_validation-0.0.2/pymatgen/io/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_common_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_for_excess_empty_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42367 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_incar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_kpoints_kspacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_potcar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/compare_to_MP_ehull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15892 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/vasp_defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    27016 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/tests/test_validation.py
```

### Comparing `pymatgen-io-validation-0.0.1/LICENSE` & `pymatgen_io_validation-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen-io-validation-0.0.1/PKG-INFO` & `pymatgen_io_validation-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,137 +1,121 @@
-Metadata-Version: 2.1
-Name: pymatgen-io-validation
-Version: 0.0.1
-Summary: A comprehensive I/O validator for electronic structure calculations
-Home-page: https://github.com/matthewkuner/pymatgen-io-validation
-Author: Matthew Kuner, Janosh Riebesell, Jason Munro, Aaron Kaplan
-Author-email: matthewkuner@berkeley.edu
-Maintainer: Matthew Kuner
-License: BSD
-Description: pymatgen-io-validation
-        =====
-        
-        This package is an extension to `pymatgen` for performing I/O validation. Specifically, this package checks for discrepancies between a specific calculation and a provided input set; it also checks for known bugs when certain input parameters are used in combination, alongside several other small checks. The initial motivation for creating this package was to validate VASP calculations performed by groups outside of the Materials Project (MP), enabling their raw data to be included in the MP Database.
-        
-        
-        Usage
-        =====
-        
-        For validating calculations from the raw files, run:
-        ```
-        from pymatgen.io.validation import ValidationDoc
-        validation_doc = ValidationDoc.from_directory(dir_name = path_to_vasp_calculation_directory)
-        ```
-        
-        In the above case, whether a calculation passes the validator can be accessed via `validation_doc.valid`. Moreover, reasons for an invalidated calculation can be accessed via `validation_doc.reasons` (this will be empty for valid calculations). Last but not least, warnings for potential issues (sometimes minor, sometimes major) can be accessed via `validation_doc.warnings`.
-        \
-        \
-        For validating calculations from `TaskDoc` objects from the [Emmet](https://github.com/materialsproject/emmet) package, run:
-        ```
-        from pymatgen.io.validation import ValidationDoc
-        validation_doc = ValidationDoc.from_task_doc(task_doc = my_task_doc)
-        ```
-        
-        Contributors
-        =====
-        
-        * [Matthew Kuner](https://github.com/matthewkuner) (lead), email: matthewkuner@gmail.com
-        * [Aaron Kaplan](https://github.com/esoteric-ephemera)
-        * [Janosh Riebesell](https://github.com/janosh)
-        * [Jason Munro](https://github.com/munrojm)
-        
-        
-        Rationale
-        ====
-        
-        | **Parameter** | **Reason** |
-        | ---- | ---- |
-        | ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states “please do not use this tag [ADDGRID] as default in all your calculations!”. ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
-        | AEXX / AMGGAX / AMGGAC / AGGAX / ALDAC / ALDAX | These parameters should be the VASP defaults unless otherwise specified in a given MP input set, as changing them is effectively a change to the level of theory. |
-        | ALGO / IALGO | ALGO must be one of: "Normal", "Conjugate", "All", "Fast", "Exact". (This corresponds to an IALGO of 38, 58, 58, 68, 90, respectively). |
-        | DEPER / EBREAK / WEIMIN | DEPER, EBREAK, and WEIMIN should not be changed according to the VASP wiki, hence MP requires them to remain as their default values. |
-        | EDIFF | EDIFF must be equal to or greater than the value in the relevant MP input set. This will ensure compatibility between results with those in the MP Database. |
-        | EDIFFG | Should be the same or better than in the relevant MP input set. For MP input sets with an energy-based cutoff, the calculation must have an energy change between the last two steps be less in magnitude than the specified EDIFFG (so even if your calculation uses force-based convergence, the energy must converge within the MP input set’s specification). The same logic applies to MP input sets with force-based EDIFFG settings. |
-        | EFERMI | EFERMI must be one of: "LEGACY", "MIDGAP" |
-        | EFIELD | Current MP input sets used to construct the main MP database do not set EFIELD, and hence we require this to be unset or set to 0. |
-        | ENAUG | If ENAUG is present in the relevant MP input set, then a calculation’s ENAUG must be equal to or better than that value. |
-        | ENCUT | ENCUT must be equal to or greater than the value in the relevant MP input set, as otherwise results will likely be incompatible with MP. |
-        | ENINI | ENINI must not be adjusted for high-throughput calculations, and hence should be left equal to the value used for ENCUT in the relevant MP input set. Values greater than the ENCUT in the relevant MP input set will also be accepted, though we expect this to be uncommon and do not recommend it. |
-        | EPSILON | EPSILON must be set to the VASP default of 1. Changing the dielectric constant of the medium will cause results to be incompatible with MP. |
-        | GGA / METAGGA | The level of theory used must match the relevant MP input set. Moreover, GGA and METAGGA should never be set simultaneously, as this has been shown to result in seriously erroneous results. See https://github.com/materialsproject/atomate2/issues/453#issuecomment-1699605867 for more details. |
-        | GGA_COMPAT | GGA_COMPAT must be set to the VASP default of True. The VASP manual only recommends setting this to False for noncollinear magnetic calculations, which are not currently included in the MP database. |
-        | IBRION | IBRION values must be one of: -1, 1, 2. Other IBRION values correspond to non-standard forms of DFT calculations that are not included in the MP database. (Note that, while phonon data is included in the MP database, such values are not calculated using, say, IBRION = 5. Such logic applies to all other IBRION values not allowed). |
-        | ICHARG | ICHARG must be set to be compatible with the calculation type. For example, if the relevant MP input set is for a SCF calculation, ICHARG $\leq 9$ must be used. For NSCF calculations, the value for ICHARG must exactly match the value contained in the relevant MP input set. |
-        | ICORELEVEL | ICORELEVEL must be set to 0. MP does not explicitly calculate core energies. |
-        | IDIPOL | IDIPOL must be set to 0 (the VASP default). |
-        | IMAGES | IMAGES must be set to 0 to match MP calculations. |
-        | INIWAV | INIWAV must be set as the VASP default of 1 to be consistent with MP calculations. |
-        | ISPIN | All values of ISPIN are allowed, though it should be noted that virtually all MP calculations permit spin symmetry breaking, and have ferromagnetic, antiferrogmanetic, or nonmagnetic ordering. |
-        | ISMEAR | The appropriate ISMEAR depends on the bandgap of the material (which cannot be known a priori). As per the VASP manual: for metals (bandgap = 0), any ISMEAR value in [0, 1, 2] is acceptable. For nonmetals (bandgap > 0), any ISMEAR value in [-5, 0] is acceptable. Hence, for those who are performing normal relaxations/static calculations and want to ensure their calculations are MP-compatible, we recommend setting ISMEAR to 0. |
-        | ISIF | MP allows any ISIF $\geq 2$. This value is restricted as such simply because all ISIF values $\geq 2$ output the complete stress tensor. |
-        | ISYM | ISYM must be one of -1, 0, 1, 2, except for when the relevant MP input set uses a hybrid functional, in which case ISYM=3 is also allowed. |
-        | ISTART | ISTART must be one of: 0, 1, 2. |
-        | IVDW | IVDW must be set to 0. MP currently does not apply any vdW dispersion corrections. |
-        | IWAVPR | IWAVPR must be set to 0 (the default). VASP discourages users from setting this tag. |
-        | KGAMMA | KGAMMA must be set to True (the VASP default). This is only relevant when no KPOINTS file is used. |
-        | KSPACING / KPOINTS | The KSPACING parameter or KPOINTS file must correspond with at least 0.9 times **the number of KPOINTS in the non-symmetry-reduced Brillouin zone specified by the relevant MP input set** (i.e., not the number of points in the irreducible wedge of the first Brillouin zone). Hence, either method of specifying the KPOINTS can be chosen. This ensures that a calculation uses a comparable number of kpoints to MP. |
-        | Kpoint mesh type (for KPOINTS) | The type of Kpoint mesh must be valid for the symmetry of the crystal structure in the calculation. For example, for a hexagonal closed packed structure, one must use a $\Gamma$-centered mesh. All Kpoints generated using Pymatgen *should* be valid. |
-        | LASPH | LASPH must be set to True (this is **<u>*not*</u>** the VASP default). |
-        | LCALCEPS | LCALCEPS must be set to False (the VASP default). |
-        | LBERRY | LBERRY must be set to False (the VASP default). |
-        | LCALCPOL | LCALCPOL  must be set to False (the VASP default). |
-        | LCHIMAG | LCHIMAG must be set to False (the VASP default). |
-        | LCORR | LCORR must be set to True (the VASP default) for calculations with IALGO = 58. |
-        | LDAU / LDAUU / LDAUJ / LDAUL / LDAUTYPE | For DFT$`+U`$ calculations, all parameters corresponding to $+U$ or $+J$ corrections must exactly match those specified in the relevant MP input set. Alternatively, LDAU = False (DFT) is always acceptable. |
-        | LDIPOL | LDIPOL must be set to False (the VASP default). |
-        | LMONO | LMONO must be set to False (the VASP default). |
-        | LEFG | LEFG must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
-        | LEPSILON | LEPSILON must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
-        | LHFCALC | The value of LHFCALC should match that of the relevant MP input set, as it will otherwise result in a change in the level of theory applied in the calculation. |
-        | LHYPERFINE | LHYPERFINE must be set to False (the VASP default). |
-        | LKPROJ | LKPROJ must be set to False (the VASP default). |
-        | LKPOINTS_OPT | LKPOINTS_OPT must be set to False. |
-        | LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that “Energies should be evaluated with the default setting for LMAXPAW”. |
-        | LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the “bench_vasp_pars.docx” document in https://github.com/materialsproject/pymatgen/issues/3322. |
-        | LMAXTAU | LMAXTAU must be set to 6 (the VASP default when using LASPH = True). |
-        | LMP2LT / LSMP2LT | Both must be set to False (VASP defaults) |
-        | LNONCOLLINEAR / LSORBIT | Both must be set to False (VASP defaults) |
-        | LOCPROJ | LOCPROJ must be set to None (the VASP default). |
-        | LOPTICS | LOPTICS must be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
-        | LORBIT | LORBIT must **<u>*not*</u>** be None if the user also sets ISPIN=2, otherwise all values of LORBIT are acceptable. This is due to magnetization values not being output when ISPIN=2 and LORBIT = None are set together. |
-        | LREAL | If the LREAL in the relevant MP input set is “Auto”, then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
-        | LRPA | LRPA must be set to False (the VASP default). MP does not currently support random phase approximation (RPA) calculations. |
-        | LSPECTRAL | LSPECTRAL must be set to False (the VASP default for most calculations). |
-        | LSUBROT | LSUBROT must be set to False (the VASP default). |
-        | MAGMOM | While any initial magnetic moments are allowed, the final total magnetic moment for any given atom must be less than 5 $\mu_B$ (Bohr magnetons) (except for elements Gd and Eu, which must be less than 10 $\mu_B$). This simply serves as a filter for erroneous data. |
-        | ML_LMFF | ML_LMFF must be set to False (the VASP default). |
-        | NGX / NGY / NGZ | The values for NGX/NGY/NGZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
-        | NGFX / NGFY / NGFZ | The values for NGFX/NGFY/NGFZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
-        | NLSPLINE | NLSPLINE should be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
-        | NBANDS | NBANDS must be greater than the value $\mathrm{ceil}(\mathrm{NELECT}/2) + 1 $(minimum allowable number of bands to avoid degeneracy) and less than 4 times (minimum allowable number of bands to avoid degeneracy). For high-throughput calculations, it is generally recommended to not set this parameter directly. See https://github.com/materialsproject/custodian/issues/224 for more information. |
-        | NELECT | NELECT must not be changed from the default value VASP would use for the particular structure and pseudopotentials calculated. The easiest way to ensure that NELECT is compliant with MP data is to simply not specify NELECT in the INCAR file. |
-        | NWRITE | NWRITE must be set to be $\geq 2$ (the VASP default is 2). |
-        | POTIM | POTIM $\leq 5$. We suggest not setting POTIM in the INCAR file, and rather allowing VASP to set it to the default value of 0.5. |
-        | PSTRESS | PSTRESS must be set to exactly 0.0 (the VASP default). |
-        | PREC | PREC must be one of: "High", "Accurate". |
-        | ROPT | ROPT should be set to be less than or equal to the default ROPT value (which is set based on the PREC tag). Hence, it is recommended to not set the ROPT tag in the INCAR file. |
-        | RWIGS | RWIGS should not be set in the INCAR file. |
-        | SCALEE | SCALEE should not be set in the INCAR file. |
-        | SYMPREC | SYMPREC must be less than or equal to 1e-3 (as this is the maximum value that the Custodian package will set SYMPREC as of March 2024). For general use, we recommend leaving SYMPREC as the default generated by your desired MP input set. |
-        | SIGMA | There are several rules for setting SIGMA:  <ol> <li> SIGMA  must be $\leq 0.05$ for non-metals (bandgap $>  0$). </li> <li> SIGMA must be $\leq 0.2$ for a metal (bandgap = 0). </li> <li> For metals, the SIGMA value must be small enough that the entropy term in the energy is $\leq$ 1 meV/atom (as suggested by the VASP manual). </li> </ol> |
-        | VCA | MP data does not include Virtual Crystal Approximation (VCA) calculations from VASP. As such, this parameter should not be set. |
-        | VASP version | The following versions of VASP are allowed: 5.4.4 or $>$ 6.0.0. For example, versions $<=$ 5.4.3 are not allowed, whereas version 6.3.1 is allowed. |
-        
-Keywords: pymatgen
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
+pymatgen-io-validation
+=====
+
+This package is an extension to `pymatgen` for performing I/O validation. Specifically, this package checks for discrepancies between a specific calculation and a provided input set; it also checks for known bugs when certain input parameters are used in combination, alongside several other small checks. The motivation for creating this package was to ensure VASP calculations performed by groups outside of the Materials Project (MP) are compliant with MP data, thus enabling their raw data to be included in the MP Database.
+
+
+Installation
+=====
+
+You can install this package by simply running
+
+`pip install pymatgen-io-validation`
+
+
+Usage
+=====
+
+For validating calculations from the raw files, run:
+```
+from pymatgen.io.validation import ValidationDoc
+validation_doc = ValidationDoc.from_directory(dir_name = path_to_vasp_calculation_directory)
+```
+
+In the above case, whether a calculation passes the validator can be accessed via `validation_doc.valid`. Moreover, reasons for an invalidated calculation can be accessed via `validation_doc.reasons` (this will be empty for valid calculations). Last but not least, warnings for potential issues (sometimes minor, sometimes major) can be accessed via `validation_doc.warnings`.
+\
+\
+For validating calculations from `TaskDoc` objects from the [Emmet](https://github.com/materialsproject/emmet) package, run:
+```
+from pymatgen.io.validation import ValidationDoc
+validation_doc = ValidationDoc.from_task_doc(task_doc = my_task_doc)
+```
+
+Contributors
+=====
+
+* [Matthew Kuner](https://github.com/matthewkuner) (lead), email: matthewkuner@gmail.com
+* [Aaron Kaplan](https://github.com/esoteric-ephemera)
+* [Janosh Riebesell](https://github.com/janosh)
+* [Jason Munro](https://github.com/munrojm)
+
+
+Rationale
+====
+
+| **Parameter** | **Reason** |
+| ---- | ---- |
+| ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states “please do not use this tag [ADDGRID] as default in all your calculations!”. ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
+| AEXX / AMGGAX / AMGGAC / AGGAX / ALDAC / ALDAX | These parameters should be the VASP defaults unless otherwise specified in a given MP input set, as changing them is effectively a change to the level of theory. |
+| ALGO / IALGO | ALGO must be one of: "Normal", "Conjugate", "All", "Fast", "Exact". (This corresponds to an IALGO of 38, 58, 58, 68, 90, respectively). |
+| DEPER / EBREAK / WEIMIN | DEPER, EBREAK, and WEIMIN should not be changed according to the VASP wiki, hence MP requires them to remain as their default values. |
+| EDIFF | EDIFF must be equal to or greater than the value in the relevant MP input set. This will ensure compatibility between results with those in the MP Database. |
+| EDIFFG | Should be the same or better than in the relevant MP input set. For MP input sets with an energy-based cutoff, the calculation must have an energy change between the last two steps be less in magnitude than the specified EDIFFG (so even if your calculation uses force-based convergence, the energy must converge within the MP input set’s specification). The same logic applies to MP input sets with force-based EDIFFG settings. |
+| EFERMI | EFERMI must be one of: "LEGACY", "MIDGAP" |
+| EFIELD | Current MP input sets used to construct the main MP database do not set EFIELD, and hence we require this to be unset or set to 0. |
+| ENAUG | If ENAUG is present in the relevant MP input set, then a calculation’s ENAUG must be equal to or better than that value. |
+| ENCUT | ENCUT must be equal to or greater than the value in the relevant MP input set, as otherwise results will likely be incompatible with MP. |
+| ENINI | ENINI must not be adjusted for high-throughput calculations, and hence should be left equal to the value used for ENCUT in the relevant MP input set. Values greater than the ENCUT in the relevant MP input set will also be accepted, though we expect this to be uncommon and do not recommend it. |
+| EPSILON | EPSILON must be set to the VASP default of 1. Changing the dielectric constant of the medium will cause results to be incompatible with MP. |
+| GGA / METAGGA | The level of theory used must match the relevant MP input set. Moreover, GGA and METAGGA should never be set simultaneously, as this has been shown to result in seriously erroneous results. See https://github.com/materialsproject/atomate2/issues/453#issuecomment-1699605867 for more details. |
+| GGA_COMPAT | GGA_COMPAT must be set to the VASP default of True. The VASP manual only recommends setting this to False for noncollinear magnetic calculations, which are not currently included in the MP database. |
+| IBRION | IBRION values must be one of: -1, 1, 2. Other IBRION values correspond to non-standard forms of DFT calculations that are not included in the MP database. (Note that, while phonon data is included in the MP database, such values are not calculated using, say, IBRION = 5. Such logic applies to all other IBRION values not allowed). |
+| ICHARG | ICHARG must be set to be compatible with the calculation type. For example, if the relevant MP input set is for a SCF calculation, ICHARG $\leq 9$ must be used. For NSCF calculations, the value for ICHARG must exactly match the value contained in the relevant MP input set. |
+| ICORELEVEL | ICORELEVEL must be set to 0. MP does not explicitly calculate core energies. |
+| IDIPOL | IDIPOL must be set to 0 (the VASP default). |
+| IMAGES | IMAGES must be set to 0 to match MP calculations. |
+| INIWAV | INIWAV must be set as the VASP default of 1 to be consistent with MP calculations. |
+| ISPIN | All values of ISPIN are allowed, though it should be noted that virtually all MP calculations permit spin symmetry breaking, and have ferromagnetic, antiferrogmanetic, or nonmagnetic ordering. |
+| ISMEAR | The appropriate ISMEAR depends on the bandgap of the material (which cannot be known a priori). As per the VASP manual: for metals (bandgap = 0), any ISMEAR value in [0, 1, 2] is acceptable. For nonmetals (bandgap > 0), any ISMEAR value in [-5, 0] is acceptable. Hence, for those who are performing normal relaxations/static calculations and want to ensure their calculations are MP-compatible, we recommend setting ISMEAR to 0. |
+| ISIF | MP allows any ISIF $\geq 2$. This value is restricted as such simply because all ISIF values $\geq 2$ output the complete stress tensor. |
+| ISYM | ISYM must be one of -1, 0, 1, 2, except for when the relevant MP input set uses a hybrid functional, in which case ISYM=3 is also allowed. |
+| ISTART | ISTART must be one of: 0, 1, 2. |
+| IVDW | IVDW must be set to 0. MP currently does not apply any vdW dispersion corrections. |
+| IWAVPR | IWAVPR must be set to 0 (the default). VASP discourages users from setting this tag. |
+| KGAMMA | KGAMMA must be set to True (the VASP default). This is only relevant when no KPOINTS file is used. |
+| KSPACING / KPOINTS | The KSPACING parameter or KPOINTS file must correspond with at least 0.9 times **the number of KPOINTS in the non-symmetry-reduced Brillouin zone specified by the relevant MP input set** (i.e., not the number of points in the irreducible wedge of the first Brillouin zone). Hence, either method of specifying the KPOINTS can be chosen. This ensures that a calculation uses a comparable number of kpoints to MP. |
+| Kpoint mesh type (for KPOINTS) | The type of Kpoint mesh must be valid for the symmetry of the crystal structure in the calculation. For example, for a hexagonal closed packed structure, one must use a $\Gamma$-centered mesh. All Kpoints generated using Pymatgen *should* be valid. |
+| LASPH | LASPH must be set to True (this is **<u>*not*</u>** the VASP default). |
+| LCALCEPS | LCALCEPS must be set to False (the VASP default). |
+| LBERRY | LBERRY must be set to False (the VASP default). |
+| LCALCPOL | LCALCPOL  must be set to False (the VASP default). |
+| LCHIMAG | LCHIMAG must be set to False (the VASP default). |
+| LCORR | LCORR must be set to True (the VASP default) for calculations with IALGO = 58. |
+| LDAU / LDAUU / LDAUJ / LDAUL / LDAUTYPE | For DFT$`+U`$ calculations, all parameters corresponding to $+U$ or $+J$ corrections must exactly match those specified in the relevant MP input set. Alternatively, LDAU = False (DFT) is always acceptable. |
+| LDIPOL | LDIPOL must be set to False (the VASP default). |
+| LMONO | LMONO must be set to False (the VASP default). |
+| LEFG | LEFG must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
+| LEPSILON | LEPSILON must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
+| LHFCALC | The value of LHFCALC should match that of the relevant MP input set, as it will otherwise result in a change in the level of theory applied in the calculation. |
+| LHYPERFINE | LHYPERFINE must be set to False (the VASP default). |
+| LKPROJ | LKPROJ must be set to False (the VASP default). |
+| LKPOINTS_OPT | LKPOINTS_OPT must be set to False. |
+| LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that “Energies should be evaluated with the default setting for LMAXPAW”. |
+| LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the “bench_vasp_pars.docx” document in https://github.com/materialsproject/pymatgen/issues/3322. |
+| LMAXTAU | LMAXTAU must be set to 6 (the VASP default when using LASPH = True). |
+| LMP2LT / LSMP2LT | Both must be set to False (VASP defaults) |
+| LNONCOLLINEAR / LSORBIT | Both must be set to False (VASP defaults) |
+| LOCPROJ | LOCPROJ must be set to None (the VASP default). |
+| LOPTICS | LOPTICS must be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
+| LORBIT | LORBIT must **<u>*not*</u>** be None if the user also sets ISPIN=2, otherwise all values of LORBIT are acceptable. This is due to magnetization values not being output when ISPIN=2 and LORBIT = None are set together. |
+| LREAL | If the LREAL in the relevant MP input set is “Auto”, then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
+| LRPA | LRPA must be set to False (the VASP default). MP does not currently support random phase approximation (RPA) calculations. |
+| LSPECTRAL | LSPECTRAL must be set to False (the VASP default for most calculations). |
+| LSUBROT | LSUBROT must be set to False (the VASP default). |
+| MAGMOM | While any initial magnetic moments are allowed, the final total magnetic moment for any given atom must be less than 5 $\mu_B$ (Bohr magnetons) (except for elements Gd and Eu, which must be less than 10 $\mu_B$). This simply serves as a filter for erroneous data. |
+| ML_LMFF | ML_LMFF must be set to False (the VASP default). |
+| NGX / NGY / NGZ | The values for NGX/NGY/NGZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
+| NGFX / NGFY / NGFZ | The values for NGFX/NGFY/NGFZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
+| NLSPLINE | NLSPLINE should be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
+| NBANDS | NBANDS must be greater than the value $\mathrm{ceil}(\mathrm{NELECT}/2) + 1 $(minimum allowable number of bands to avoid degeneracy) and less than 4 times (minimum allowable number of bands to avoid degeneracy). For high-throughput calculations, it is generally recommended to not set this parameter directly. See https://github.com/materialsproject/custodian/issues/224 for more information. |
+| NELECT | NELECT must not be changed from the default value VASP would use for the particular structure and pseudopotentials calculated. The easiest way to ensure that NELECT is compliant with MP data is to simply not specify NELECT in the INCAR file. |
+| NWRITE | NWRITE must be set to be $\geq 2$ (the VASP default is 2). |
+| POTIM | POTIM $\leq 5$. We suggest not setting POTIM in the INCAR file, and rather allowing VASP to set it to the default value of 0.5. |
+| PSTRESS | PSTRESS must be set to exactly 0.0 (the VASP default). |
+| PREC | PREC must be one of: "High", "Accurate". |
+| ROPT | ROPT should be set to be less than or equal to the default ROPT value (which is set based on the PREC tag). Hence, it is recommended to not set the ROPT tag in the INCAR file. |
+| RWIGS | RWIGS should not be set in the INCAR file. |
+| SCALEE | SCALEE should not be set in the INCAR file. |
+| SYMPREC | SYMPREC must be less than or equal to 1e-3 (as this is the maximum value that the Custodian package will set SYMPREC as of March 2024). For general use, we recommend leaving SYMPREC as the default generated by your desired MP input set. |
+| SIGMA | There are several rules for setting SIGMA:  <ol> <li> SIGMA  must be $\leq 0.05$ for non-metals (bandgap $>  0$). </li> <li> SIGMA must be $\leq 0.2$ for a metal (bandgap = 0). </li> <li> For metals, the SIGMA value must be small enough that the entropy term in the energy is $\leq$ 1 meV/atom (as suggested by the VASP manual). </li> </ol> |
+| VCA | MP data does not include Virtual Crystal Approximation (VCA) calculations from VASP. As such, this parameter should not be set. |
+| VASP version | The following versions of VASP are allowed: 5.4.4 or $>$ 6.0.0. For example, versions $<=$ 5.4.3 are not allowed, whereas version 6.3.1 is allowed. |
```

### Comparing `pymatgen-io-validation-0.0.1/README.md` & `pymatgen_io_validation-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,55 @@
+Metadata-Version: 2.1
+Name: pymatgen-io-validation
+Version: 0.0.2
+Summary: A comprehensive I/O validator for electronic structure calculations
+Home-page: https://github.com/materialsproject/pymatgen-io-validation
+Author: Janosh Riebesell, Jason Munro, Aaron Kaplan
+Author-email: Matthew Kuner <matthewkuner@gmail.com>
+Maintainer: Matthew Kuner
+License: modified BSD
+Keywords: io,validation,dft,vasp
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pymatgen
+Requires-Dist: numpy
+Requires-Dist: requests
+Provides-Extra: dev
+Requires-Dist: pre-commit>=2.12.1; extra == "dev"
+Provides-Extra: tests
+Requires-Dist: pytest==8.0.2; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0; extra == "tests"
+Requires-Dist: types-requests; extra == "tests"
+
 pymatgen-io-validation
 =====
 
-This package is an extension to `pymatgen` for performing I/O validation. Specifically, this package checks for discrepancies between a specific calculation and a provided input set; it also checks for known bugs when certain input parameters are used in combination, alongside several other small checks. The initial motivation for creating this package was to validate VASP calculations performed by groups outside of the Materials Project (MP), enabling their raw data to be included in the MP Database.
+This package is an extension to `pymatgen` for performing I/O validation. Specifically, this package checks for discrepancies between a specific calculation and a provided input set; it also checks for known bugs when certain input parameters are used in combination, alongside several other small checks. The motivation for creating this package was to ensure VASP calculations performed by groups outside of the Materials Project (MP) are compliant with MP data, thus enabling their raw data to be included in the MP Database.
+
+
+Installation
+=====
+
+You can install this package by simply running
+
+`pip install pymatgen-io-validation`
 
 
 Usage
 =====
 
 For validating calculations from the raw files, run:
 ```
```

### Comparing `pymatgen-io-validation-0.0.1/examples/MP_compliant_job.py` & `pymatgen_io_validation-0.0.2/examples/MP_compliant_job.py`

 * *Files identical despite different names*

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_common_errors.py` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_common_errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,224 +2,279 @@
 
 from __future__ import annotations
 from dataclasses import dataclass, field
 import numpy as np
 
 from typing import TYPE_CHECKING
 
+from pymatgen.io.validation.common import BaseValidator
+
 if TYPE_CHECKING:
     from emmet.core.tasks import TaskDoc
+    from emmet.core.vasp.calc_types.enums import RunType
     from emmet.core.vasp.task_valid import TaskDocument
     from pymatgen.core import Structure
     from pymatgen.io.vasp import Incar
     from typing import Sequence
 
 
 @dataclass
-class CheckCommonErrors:
+class CheckCommonErrors(BaseValidator):
     """
     Check for common calculation errors.
 
     Parameters
     -----------
+    reasons : list[str]
+        A list of error strings to update if a check fails. These are higher
+        severity and would deprecate a calculation.
+    warnings : list[str]
+        A list of warning strings to update if a check fails. These are lower
+        severity and would flag a calculation for possible review.
+    task_doc : emmet.core TaskDoc | TaskDocument
+        Task document parsed from the calculation directory.
+    parameters : dict[str,Any]
+        Dict of user-supplied/-parsed INCAR parameters.
+    structure: Pymatgen Structure
+        Structure used in the calculation.
+    run_type: RunType
+        Run type of the calculation
+    name : str = "Check common errors"
+        Name of the validator
+    fast : bool = False
+        True: stop validation when any single check fails
     defaults : dict
         Dict of default parameters
     valid_max_magmoms : dict[str,float]
         Dict of maximum magmoms corresponding to a given element.
     exclude_elements : set[str]
         Set of elements that cannot be added to the Materials Project's hull.
     valid_max_allowed_scf_gradient : float
         Largest permitted change in total energies between two SCF cycles.
     num_ionic_steps_to_avg_drift_over : int
         Number of ionic steps to average over to yield the drift in total energy.
     """
 
+    reasons: list[str]
+    warnings: list[str]
+    task_doc: TaskDoc | TaskDocument = None
+    parameters: dict = None
+    structure: Structure = None
+    run_type: RunType = None
+    name: str = "Check common errors"
+    fast: bool = False
     defaults: dict | None = None
     # TODO: make this also work for elements Gd and Eu, which have magmoms >5 in at least one of their pure structures
     valid_max_magmoms: dict[str, float] = field(default_factory=lambda: {"Gd": 10.0, "Eu": 10.0})
     exclude_elements: set[str] = field(default_factory=lambda: {"Am", "Po"})
     valid_max_allowed_scf_gradient: float | None = None
     num_ionic_steps_to_avg_drift_over: int | None = None
 
-    def check(
-        self,
-        reasons: list[str],
-        warnings: list[str],
-        task_doc: TaskDoc | TaskDocument,
-        parameters: dict,
-        structure: Structure,
-    ) -> None:
-        """
-        Check for common calculation errors.
+    def __post_init__(self):
+        self.incar = self.task_doc["calcs_reversed"][0]["input"]["incar"]
+        self.ionic_steps = self.task_doc["calcs_reversed"][0]["output"]["ionic_steps"]
+
+    def _check_run_type(self) -> None:
+        if f"{self.run_type}".upper() not in {"GGA", "GGA+U", "PBE", "PBE+U", "R2SCAN"}:
+            self.reasons.append(f"FUNCTIONAL --> Functional {self.run_type} not currently accepted.")
+
+    def _check_parse(self) -> None:
+        if self.parameters == {} or self.parameters is None:
+            self.reasons.append(
+                "CAN NOT PROPERLY PARSE CALCULATION --> Issue parsing input parameters from the vasprun.xml file."
+            )
 
-        Parameters
-        -----------
-        reasons : list[str]
-            A list of error strings to update if a check fails. These are higher
-            severity and would deprecate a calculation.
-        warnings : list[str]
-            A list of warning strings to update if a check fails. These are lower
-            severity and would flag a calculation for possible review.
-        task_doc : emmet.core TaskDoc | TaskDocument
-            Task document parsed from the calculation directory.
-        parameters : dict[str,Any]
-            Dict of user-supplied/-parsed INCAR parameters.
-        structure: Pymatgen Structure
-            Structure used in the calculation.
-        """
+    def _check_gga_and_metagga(self) -> None:
 
-        task_doc = task_doc.model_dump()
-        incar = task_doc["calcs_reversed"][0]["input"]["incar"]
         # Check for cases where both GGA and METAGGA are set. This should *not* be allowed, as it can erroneously change
         # the outputted energy significantly. See https://github.com/materialsproject/atomate2/issues/453#issuecomment-1699605867
         # for more details.
-        if incar.get("GGA", "--") != "--" and str(incar.get("METAGGA", None)).lower() not in ["--", "none"]:
-            reasons.append(
+        if self.incar.get("GGA", "--") != "--" and str(self.incar.get("METAGGA", None)).lower() not in {"--", "none"}:
+            self.reasons.append(
                 "KNOWN BUG --> GGA and METAGGA should never be specified together, as this can cause major errors in the "
                 "outputted energy. See https://github.com/materialsproject/atomate2/issues/453#issuecomment-1699605867 "
                 "for more information."
             )
 
+    def _check_electronic_convergence(self) -> None:
         # check if structure electronically converged
-        ionic_steps = task_doc["calcs_reversed"][0]["output"]["ionic_steps"]
-        final_esteps = (
-            ionic_steps[-1]["electronic_steps"]
-            if incar.get("ALGO", self.defaults["ALGO"]["value"]).lower() != "chi"
-            else 0
-        )
-        # In a response function run there is no ionic steps, there is no scf step
-        if parameters.get("LEPSILON", self.defaults["LEPSILON"]["value"]):
-            i = 1
-            to_check = {"e_wo_entrp", "e_fr_energy", "e_0_energy"}
-            while set(final_esteps[i]) == to_check:
-                i += 1
-            is_converged = i + 1 != parameters.get("NELM", self.defaults["NELM"]["value"])
-        else:
-            is_converged = len(final_esteps) < parameters.get("NELM", self.defaults["NELM"]["value"])
 
-        if not is_converged:
-            reasons.append(
-                "CONVERGENCE --> Did not achieve electronic convergence in the final ionic step. NELM should be increased."
-            )
+        if self.incar.get("ALGO", self.defaults["ALGO"]["value"]).lower() != "chi":
+            # Response function calculations are non-self-consistent: only one ionic step, no electronic SCF
+            if self.parameters.get("LEPSILON", self.defaults["LEPSILON"]["value"]):
+
+                final_esteps = self.ionic_steps[-1]["electronic_steps"]
+                to_check = {"e_wo_entrp", "e_fr_energy", "e_0_energy"}
+
+                for i in range(len(final_esteps)):
+                    if set(final_esteps[i]) != to_check:
+                        break
+                    i += 1
+
+                is_converged = i + 1 < self.parameters.get("NELM", self.defaults["NELM"]["value"])
+                n_non_conv = 1
+
+            else:
+                conv_steps = [
+                    len(self.ionic_steps[i]["electronic_steps"])
+                    < self.parameters.get("NELM", self.defaults["NELM"]["value"])
+                    for i in range(len(self.ionic_steps))
+                ]
+                is_converged = all(conv_steps)
+                n_non_conv = len([step for step in conv_steps if not step])
+
+            if not is_converged:
+                self.reasons.append(
+                    f"CONVERGENCE --> Did not achieve electronic convergence in {n_non_conv} ionic step(s). NELM should be increased."
+                )
 
+    def _check_drift_forces(self) -> None:
         # Check if drift force is too large
         try:
-            all_drift_forces = task_doc["calcs_reversed"][0]["output"]["outcar"]["drift"]
+            all_drift_forces = self.task_doc["calcs_reversed"][0]["output"]["outcar"]["drift"]
             if len(all_drift_forces) < self.num_ionic_steps_to_avg_drift_over:
                 drift_forces_to_avg_over = all_drift_forces
             else:
                 drift_forces_to_avg_over = all_drift_forces[::-1][: self.num_ionic_steps_to_avg_drift_over]
 
             drift_mags_to_avg_over = [np.linalg.norm(drift_forces) for drift_forces in drift_forces_to_avg_over]
             cur_avg_drift_mag = np.average(drift_mags_to_avg_over)
 
             valid_max_drift = 0.05
             if cur_avg_drift_mag > valid_max_drift:
-                reasons.append(
+                self.reasons.append(
                     f"CONVERGENCE --> Excessive drift of {round(cur_avg_drift_mag,4)} eV/A is greater than allowed "
                     f"value of {valid_max_drift} eV/A."
                 )
         except Exception:
-            warnings.append("Drift forces not contained in calcs_reversed! Can not check for excessive drift.")
+            self.warnings.append("Drift forces not contained in calcs_reversed! Can not check for excessive drift.")
 
+    def _check_positive_energy(self) -> None:
         # Check for excessively positive final energies (which usually indicates a bad structure)
         valid_max_energy_per_atom = 50
-        cur_final_energy_per_atom = task_doc["output"]["energy_per_atom"]
+        cur_final_energy_per_atom = self.task_doc["output"]["energy_per_atom"]
         if cur_final_energy_per_atom > valid_max_energy_per_atom:
-            reasons.append(
+            self.reasons.append(
                 f"LARGE POSITIVE FINAL ENERGY --> Final energy is {round(cur_final_energy_per_atom,4)} eV/atom, which is "
                 f"greater than the maximum allowed value of {valid_max_energy_per_atom} eV/atom."
             )
 
+    def _check_large_magmoms(self) -> None:
         # Check for excessively large final magnetic moments
-        cur_magmoms = [abs(mag["tot"]) for mag in task_doc["calcs_reversed"][0]["output"]["outcar"]["magnetization"]]
+        cur_magmoms = [
+            abs(mag["tot"]) for mag in self.task_doc["calcs_reversed"][0]["output"]["outcar"]["magnetization"]
+        ]
         bad_site_magmom_msgs = []
         if len(cur_magmoms) > 0:
-            for site_num in range(0, len(structure)):
-                cur_site_ele = structure.sites[site_num].species_string
+            for site_num in range(0, len(self.structure)):
+                cur_site_ele = self.structure.sites[site_num].species_string
                 cur_site_magmom = cur_magmoms[site_num]
                 cur_site_max_allowed_magmom = self.valid_max_magmoms.get(cur_site_ele, 5.0)
 
                 if cur_site_magmom > cur_site_max_allowed_magmom:
                     bad_site_magmom_msgs.append(
                         f"at least one {cur_site_ele} site with magmom greater than {cur_site_max_allowed_magmom}"
                     )
+
         if len(bad_site_magmom_msgs) > 0:
-            reasons.append(
+            self.reasons.append(
                 "MAGNETISM --> Final structure contains sites with magnetic moments "
                 "that are very likely erroneous. This includes: "
                 f"{'; '.join(set(bad_site_magmom_msgs))}."
             )
 
+    def _check_scf_grad(self) -> None:
         # Check for a SCF gradient that is too large (usually indicates unstable calculations)
         # NOTE: do NOT use `e_0_energy`, as there is a bug in the vasprun.xml when printing that variable
         # (see https://www.vasp.at/forum/viewtopic.php?t=16942 for more details).
-        skip = abs(parameters.get("NELMDL", self.defaults["NELMDL"]["value"])) - 1
-        energies = [d["e_fr_energy"] for d in ionic_steps[-1]["electronic_steps"]]
+        skip = abs(self.parameters.get("NELMDL", self.defaults["NELMDL"]["value"])) - 1
+        energies = [d["e_fr_energy"] for d in self.ionic_steps[-1]["electronic_steps"]]
         if len(energies) > skip:
             cur_max_gradient = np.max(np.gradient(energies)[skip:])
-            cur_max_gradient_per_atom = cur_max_gradient / structure.num_sites
+            cur_max_gradient_per_atom = cur_max_gradient / self.structure.num_sites
             if cur_max_gradient_per_atom > self.valid_max_allowed_scf_gradient:
-                warnings.append(
+                self.warnings.append(
                     f"STABILITY --> The max SCF gradient is {round(cur_max_gradient_per_atom,4)} eV/atom, "
                     "which is larger than the typical max expected value of "
                     f"{self.valid_max_allowed_scf_gradient} eV/atom. "
                     f"This sometimes indicates an unstable calculation."
                 )
         else:
-            warnings.append(
-                "Not enough electronic steps to compute valid gradient" " and compare with max SCF gradient tolerance."
+            self.warnings.append(
+                "Not enough electronic steps to compute valid gradient and compare with max SCF gradient tolerance."
             )
 
+    def _check_unused_elements(self) -> None:
         # Check for Am and Po elements. These currently do not have proper elemental entries
         # and will not get treated properly by the thermo builder.
-        elements = set(task_doc["chemsys"].split("-"))
+        elements = set(self.task_doc["chemsys"].split("-"))
         if excluded_elements := self.exclude_elements.intersection(elements):
-            reasons.append(
+            self.reasons.append(
                 f"COMPOSITION --> Your structure contains the elements {' '.join(excluded_elements)}, "
                 "which are not currently being accepted."
             )
 
 
 @dataclass
-class CheckVaspVersion:
+class CheckVaspVersion(BaseValidator):
     """
     Check for common errors related to the version of VASP used.
 
     Parameters
     -----------
+    reasons : list[str]
+        A list of error strings to update if a check fails. These are higher
+        severity and would deprecate a calculation.
+    warnings : list[str]
+        A list of warning strings to update if a check fails. These are lower
+        severity and would flag a calculation for possible review.
+    vasp_version: Sequence[int]
+        Vasp version, e.g., 6.4.1 could be represented as (6,4,1)
+    parameters : dict[str,Any]
+        Dict of user-supplied/-parsed INCAR parameters.
+    incar : dict | Incar
+        INCAR corresponding to the calculation.
+    name : str = "Base validator class"
+        Name of the validator class
+    fast : bool = False
+        Whether to perform quick check.
+        True: stop validation if any check fails.
+        False: perform all checks.
     defaults : dict
         Dict of default parameters
     """
 
+    reasons: list[str]
+    warnings: list[str]
+    vasp_version: Sequence[int] = None
+    parameters: dict = None
+    incar: dict | Incar = None
+    name: str = "VASP version validator"
     defaults: dict | None = None
 
-    def check(self, reasons: list[str], vasp_version: Sequence[int], parameters: dict, incar: dict | Incar) -> None:
+    def _check_vasp_version(self) -> None:
         """
         Check for common errors related to the version of VASP used.
 
         reasons : list[str]
             A list of error strings to update if a check fails. These are higher
             severity and would deprecate a calculation.
-        vasp_version: Sequence[int]
-            Vasp version, e.g., 6.4.1 could be represented as (6,4,1)
-        parameters : dict[str,Any]
-            Dict of user-supplied/-parsed INCAR parameters.
-        incar : dict | Incar
-            INCAR corresponding to the calculation.
+        warnings : list[str]
+            A list of warning strings to update if a check fails. These are lower
+            severity and would flag a calculation for possible review.
         """
         if (
-            vasp_version[0] == 5
-            and (incar.get("METAGGA", self.defaults["METAGGA"]["value"]) not in [None, "--", "None"])
-            and parameters.get("ISPIN", self.defaults["ISPIN"]["value"]) == 2
+            self.vasp_version[0] == 5
+            and (self.incar.get("METAGGA", self.defaults["METAGGA"]["value"]) not in [None, "--", "None"])
+            and self.parameters.get("ISPIN", self.defaults["ISPIN"]["value"]) == 2
         ):
-            reasons.append(
+            self.reasons.append(
                 "POTENTIAL BUG --> We believe that there may be a bug with spin-polarized calculations for METAGGAs "
                 "in some versions of VASP 5. Please create a new GitHub issue if you believe this "
                 "is not the case and we will consider changing this check!"
             )
-        elif (list(vasp_version) != [5, 4, 4]) and (vasp_version[0] < 6):
-            vasp_version_str = ".".join([str(x) for x in vasp_version])
-            reasons.append(
+        elif (list(self.vasp_version) != [5, 4, 4]) and (self.vasp_version[0] < 6):
+            vasp_version_str = ".".join([str(x) for x in self.vasp_version])
+            self.reasons.append(
                 f"VASP VERSION --> This calculation is using VASP version {vasp_version_str}, "
                 "but we only allow versions 5.4.4 and >=6.0.0 (as of July 2023)."
             )
```

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_for_excess_empty_space.py` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_for_excess_empty_space.py`

 * *Files identical despite different names*

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_incar.py` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_incar.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,127 +3,132 @@
 from __future__ import annotations
 import copy
 from dataclasses import dataclass
 from math import isclose
 import numpy as np
 from emmet.core.vasp.calc_types.enums import TaskType
 
+from pymatgen.io.validation.common import BaseValidator
+
 from typing import TYPE_CHECKING, Literal
 
 if TYPE_CHECKING:
-    from emmet.core.vasp.task_valid import TaskDocument
-    from emmet.core.tasks import TaskDoc
     from typing import Any, Sequence
     from pymatgen.core import Structure
     from pymatgen.io.vasp.sets import VaspInputSet
 
 # TODO: fix ISIF getting overwritten by MP input set.
 
 
 @dataclass
-class CheckIncar:
+class CheckIncar(BaseValidator):
     """
     Check calculation parameters related to INCAR input tags.
 
+    Because this class checks many INCAR tags in sequence, while it
+    inherits from the `pymatgen.io.validation.common.BaseValidator`
+    class, it also defines a custom `check` method.
+
+    reasons : list[str]
+        A list of error strings to update if a check fails. These are higher
+        severity and would deprecate a calculation.
+    warnings : list[str]
+        A list of warning strings to update if a check fails. These are lower
+        severity and would flag a calculation for possible review.
+    valid_input_set: VaspInputSet
+        Valid input set to compare user INCAR parameters to.
+    task_doc : dict
+        Task document parsed from the calculation directory, as a dict
+    parameters : dict[str,Any]
+        Dict of user-supplied/-parsed INCAR parameters.
+    structure: Pymatgen Structure
+        Structure used in the calculation.
+    vasp_version: Sequence[int]
+        Vasp version, e.g., 6.4.1 could be represented as (6,4,1)
+    task_type : TaskType
+        Task type of the calculation.
+    name : str = "Check INCAR tags"
+        Name of the validator.
     defaults : dict
         Dict of default parameters.
     fft_grid_tolerance: float
         Directly calculating the FFT grid defaults from VASP is actually impossible
         without information on how VASP was compiled. This is because the FFT
         params generated depend on whatever fft library used. So instead, we do our
         best to calculate the FFT grid defaults and then lower it artificially by
         `fft_grid_tolerance`. So if the user's FFT grid parameters are greater than
         (fft_grid_tolerance x slightly-off defaults), the FFT params are marked
         as valid.
     """
 
+    reasons: list[str]
+    warnings: list[str]
+    valid_input_set: VaspInputSet = None
+    task_doc: dict = None
+    parameters: dict[str, Any] = None
+    structure: Structure = None
+    vasp_version: Sequence[int] = None
+    task_type: TaskType = None
+    name: str = "Check INCAR tags"
     defaults: dict | None = None
     fft_grid_tolerance: float | None = None
 
-    def check(
-        self,
-        reasons: list[str],
-        warnings: list[str],
-        valid_input_set: VaspInputSet,
-        task_doc: TaskDoc | TaskDocument,
-        parameters: dict[str, Any],
-        structure: Structure,
-        vasp_version: Sequence[int],
-        task_type: TaskType,
-    ) -> None:
+    def check(self) -> None:
         """
         Check calculation parameters related to INCAR input tags.
 
         This first updates any parameter with a specified update method.
         In practice, each INCAR tag in `vasp_defaults.yaml` has a "tag"
         attribute. If there is an update method
         `UpdateParameterValues.update_{tag.replace(" ","_")}_params`,
         all parameters with that tag will be updated.
 
         Then after all missing values in the supplied parameters (padding
         implicit values with their defaults), this checks whether the user-
         supplied/-parsed parameters satisfy a set of operations against the
         reference valid input set.
-
-        Parameters
-        -----------
-        reasons : list[str]
-            A list of error strings to update if a check fails. These are higher
-            severity and would deprecate a calculation.
-        warnings : list[str]
-            A list of warning strings to update if a check fails. These are lower
-            severity and would flag a calculation for possible review.
-        valid_input_set: VaspInputSet
-            Valid input set to compare user INCAR parameters to.
-        task_doc : emmet.core TaskDoc | TaskDocument
-            Task document parsed from the calculation directory.
-        parameters : dict[str,Any]
-            Dict of user-supplied/-parsed INCAR parameters.
-        structure: Pymatgen Structure
-            Structure used in the calculation.
-        vasp_version: Sequence[int]
-            Vasp version, e.g., 6.4.1 could be represented as (6,4,1)
-        task_type : TaskType
-            Task type of the calculation.
         """
 
         # Instantiate class that updates "dynamic" INCAR tags
         # (like NBANDS, or hybrid-related parameters)
 
         working_params = UpdateParameterValues(
-            parameters=parameters,
+            parameters=self.parameters,
             defaults=self.defaults,
-            input_set=valid_input_set,
-            structure=structure,
-            task_doc=task_doc,
-            vasp_version=vasp_version,
-            task_type=task_type,
+            input_set=self.valid_input_set,
+            structure=self.structure,
+            task_doc=self.task_doc,
+            vasp_version=self.vasp_version,
+            task_type=self.task_type,
             fft_grid_tolerance=self.fft_grid_tolerance,
         )
         # Update values in the working parameters by adding
         # defaults to unspecified INCAR tags, and by updating
         # any INCAR tag that has a specified update method
         working_params.update_parameters_and_defaults()
 
         # Validate each parameter in the set of working parameters
         simple_validator = BasicValidator()
         for key in working_params.defaults:
+
+            if self.fast and len(self.reasons) > 0:
+                # fast check: stop checking whenever a single check fails
+                break
+
             simple_validator.check_parameter(
-                reasons=reasons,
-                warnings=warnings,
+                reasons=self.reasons,
+                warnings=self.warnings,
                 input_tag=working_params.defaults[key].get("alias", key),
                 current_values=working_params.parameters[key],
                 reference_values=working_params.valid_values[key],
                 operations=working_params.defaults[key]["operation"],
                 tolerance=working_params.defaults[key]["tolerance"],
                 append_comments=working_params.defaults[key]["comment"],
                 severity=working_params.defaults[key]["severity"],
             )
-            # if key == "ISIF":
-            #    print("batz",key,working_params.parameters[key], parameters.get("ISIF"),working_params.valid_values[key],working_params.defaults[key])
 
 
 class UpdateParameterValues:
     """
     Update a set of parameters according to supplied rules and defaults.
 
     While many of the parameters in VASP need only a simple check to determine
@@ -162,15 +167,15 @@
 
     def __init__(
         self,
         parameters: dict[str, Any],
         defaults: dict[str, dict],
         input_set: VaspInputSet,
         structure: Structure,
-        task_doc: TaskDoc | TaskDocument,
+        task_doc: dict,
         vasp_version: Sequence[int],
         task_type: TaskType,
         fft_grid_tolerance: float,
     ) -> None:
         """
         Given a set of user parameters, a valid input set, and defaults, update certain tagged parameters.
 
@@ -180,16 +185,16 @@
             Dict of user-supplied parameters.
         defaults: dict
             Dict of default values for parameters, tags for parameters, and the operation to check them.
         input_set: VaspInputSet
             Valid input set to compare parameters to.
         structure: Pymatgen Structure
             Structure used in the calculation.
-        task_doc : emmet.core TaskDoc | TaskDocument
-            Task document parsed from the calculation directory.
+        task_doc : dict
+            Task document parsed from the calculation directory, as a dict
         vasp_version: Sequence[int]
             Vasp version, e.g., 6.4.1 could be represented as (6,4,1)
         task_type : TaskType
             Task type of the calculation.
         fft_grid_tolerance: float
             See docstr for `_check_incar`. The FFT grid generation has been udpated frequently
             in VASP, and determining the grid density with absolute certainty is not possible.
@@ -199,16 +204,15 @@
         self.parameters = copy.deepcopy(parameters)
         self.defaults = copy.deepcopy(defaults)
         self.input_set = input_set
         self.vasp_version = vasp_version
         self.structure = structure
         self.valid_values: dict[str, Any] = {}
 
-        # convert to dict for consistent handling of attrs
-        self.task_doc = task_doc.model_dump()
+        self.task_doc = task_doc
         # Add some underscored values for convenience
         self._fft_grid_tolerance = fft_grid_tolerance
         self._calcs_reversed = self.task_doc["calcs_reversed"]
         self._incar = self._calcs_reversed[0]["input"]["incar"]
         self._ionic_steps = self._calcs_reversed[0]["output"]["ionic_steps"]
         self._nionic_steps = len(self._ionic_steps)
         self._potcar = self._calcs_reversed[0]["input"]["potcar_spec"]
@@ -227,15 +231,15 @@
         # add defaults to parameters from the incar as needed
         self.add_defaults_to_parameters(valid_values_source=self.input_set.incar)
         # collect list of tags in parameter defaults
         for tag in tag_order:
             # check to see if update method for that tag exists, and if so, run it
             update_method_str = f"update_{tag}_params"
             if hasattr(self, update_method_str):
-                self.__getattribute__(update_method_str)()
+                getattr(self, update_method_str)()
 
         # add defaults to parameters from the defaults as needed
         self.add_defaults_to_parameters()
 
         for key in self.defaults:
             for attr in self._default_schema:
                 self.defaults[key][attr] = self.defaults[key].get(attr, self._default_schema[attr])
@@ -868,15 +872,16 @@
         if operation == "approx" and isinstance(current_value, float):
             kwargs.update({"rel_tol": tolerance or self.tolerance, "abs_tol": 0.0})
         valid_value = self._comparator(current_value, operation, reference_value, **kwargs)
 
         if not valid_value:
             error_list.append(
                 f"INPUT SETTINGS --> {input_tag}: is {current_value}, but should be "
-                f"{operation} {reference_value}. {append_comments}"
+                f"{'' if operation == 'auto fail' else operation + ' '}{reference_value}."
+                f"{' ' if len(append_comments) > 0 else ''}{append_comments}"
             )
 
     def check_parameter(
         self,
         reasons: list[str],
         warnings: list[str],
         input_tag: str,
```

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_kpoints_kspacing.py` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_kpoints_kspacing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,140 @@
 """Validate VASP KPOINTS files or the KSPACING/KGAMMA INCAR settings."""
 
 from __future__ import annotations
 from dataclasses import dataclass
 import numpy as np
 from pymatgen.io.vasp import Kpoints
 
+from pymatgen.io.validation.common import BaseValidator
+
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pymatgen.core import Structure
     from pymatgen.io.vasp.sets import VaspInputSet
 
 
 @dataclass
-class CheckKpointsKspacing:
+class CheckKpointsKspacing(BaseValidator):
     """
     Check that k-point density is sufficiently high and is compatible with lattice symmetry.
 
     Parameters
     -----------
+    reasons : list[str]
+        A list of error strings to update if a check fails. These are higher
+        severity and would deprecate a calculation.
+    warnings : list[str]
+        A list of warning strings to update if a check fails. These are lower
+        severity and would flag a calculation for possible review.
+    valid_input_set: VaspInputSet
+        Valid input set to compare user INCAR parameters to.
+    kpoints : Kpoints or dict
+        Kpoints object or its .as_dict() representation used in the calculation.
+    structure : pymatgen.core.Structure
+        The structure used in the calculation
+    name : str = "Check k-point density"
+        Name of the validator class
+    fast : bool = False
+        Whether to perform quick check.
+        True: stop validation if any check fails.
+        False: perform all checks.
     defaults : dict
         Dict of default parameters
     kpts_tolerance : float
         Tolerance for evaluating k-point density, as the k-point generation
         scheme is inconsistent across VASP versions
     allow_explicit_kpoint_mesh : str | bool
         Whether to permit explicit generation of k-points (as for a bandstructure calculation).
     allow_kpoint_shifts : bool
         Whether to permit shifting the origin of the k-point mesh from Gamma.
     """
 
+    reasons: list[str]
+    warnings: list[str]
+    name: str = "Check k-point density"
+    valid_input_set: VaspInputSet = None
+    kpoints: Kpoints | dict = None
+    structure: Structure = None
     defaults: dict | None = None
     kpts_tolerance: float | None = None
     allow_explicit_kpoint_mesh: str | bool = False
     allow_kpoint_shifts: bool = False
 
-    def _get_valid_num_kpts(self, valid_input_set: VaspInputSet, structure: Structure) -> int:
+    def _get_valid_num_kpts(self) -> int:
         """
         Get the minimum permitted number of k-points for a structure according to an input set.
 
-        Parameters
-        -----------
-        valid_input_set: VaspInputSet
-            Valid input set to compare user INCAR parameters to.
-        structure : pymatgen.core.Structure
-            The structure used in the calculation
-
         Returns
         -----------
-        int, the minimum permitted number of k-points.
+        int, the minimum permitted number of k-points, consistent with self.kpts_tolerance
         """
         # If MP input set specifies KSPACING in the INCAR
-        if ("KSPACING" in valid_input_set.incar.keys()) and (valid_input_set.kpoints is None):
-            valid_kspacing = valid_input_set.incar.get("KSPACING", self.defaults["KSPACING"]["value"])
-            latt_cur_anorm = structure.lattice.abc
+        if ("KSPACING" in self.valid_input_set.incar.keys()) and (self.valid_input_set.kpoints is None):
+            valid_kspacing = self.valid_input_set.incar.get("KSPACING", self.defaults["KSPACING"]["value"])
+            latt_cur_anorm = self.structure.lattice.abc
             # number of kpoints along each of the three lattice vectors
             nk = [max(1, np.ceil(2 * np.pi / (valid_kspacing * latt_cur_anorm[ik]))) for ik in range(3)]
             valid_num_kpts = np.prod(nk)
         # If MP input set specifies a KPOINTS file
         else:
-            valid_num_kpts = valid_input_set.kpoints.num_kpts or np.prod(valid_input_set.kpoints.kpts[0])
+            valid_num_kpts = self.valid_input_set.kpoints.num_kpts or np.prod(self.valid_input_set.kpoints.kpts[0])
+
+        return int(np.floor(int(valid_num_kpts) * self.kpts_tolerance))
+
+    def _check_user_shifted_mesh(self) -> None:
+        # Check for user shifts
+        if (not self.allow_kpoint_shifts) and any(shift_val != 0 for shift_val in self.kpoints["usershift"]):
+            self.reasons.append("INPUT SETTINGS --> KPOINTS: shifting the kpoint mesh is not currently allowed.")
 
-        return int(valid_num_kpts)
+    def _check_explicit_mesh_permitted(self) -> None:
+        # Check for explicit kpoint meshes
+
+        if (not self.allow_explicit_kpoint_mesh) and len(self.kpoints["kpoints"]) > 1:
+            self.reasons.append(
+                "INPUT SETTINGS --> KPOINTS: explicitly defining "
+                "the k-point mesh is not currently allowed. "
+                "Automatic k-point generation is required."
+            )
 
-    def check(
-        self, reasons: list[str], valid_input_set: VaspInputSet, kpoints: Kpoints | dict, structure: Structure
-    ) -> None:
+    def _check_kpoint_density(self) -> None:
         """
         Check that k-point density is sufficiently high and is compatible with lattice symmetry.
-
-        Parameters
-        -----------
-        reasons : list[str]
-            A list of error strings to update if a check fails. These are higher
-            severity and would deprecate a calculation.
-        valid_input_set: VaspInputSet
-            Valid input set to compare user INCAR parameters to.
-        kpoints : Kpoints or dict
-            Kpoints object or its .as_dict() representation used in the calculation.
-        structure : pymatgen.core.Structure
-            The structure used in the calculation
         """
 
         # Check number of kpoints used
-        valid_num_kpts = self._get_valid_num_kpts(valid_input_set, structure)
-        valid_num_kpts = int(np.floor(valid_num_kpts * self.kpts_tolerance))
+        valid_num_kpts = self._get_valid_num_kpts()
 
-        if isinstance(kpoints, Kpoints):
-            kpoints = kpoints.as_dict()
+        if isinstance(self.kpoints, Kpoints):
+            self.kpoints = self.kpoints.as_dict()
 
-        cur_num_kpts = max(kpoints.get("nkpoints", 0), np.prod(kpoints.get("kpoints")), len(kpoints.get("kpoints")))
+        cur_num_kpts = max(
+            self.kpoints.get("nkpoints", 0), np.prod(self.kpoints.get("kpoints")), len(self.kpoints.get("kpoints"))
+        )
         if cur_num_kpts < valid_num_kpts:
-            reasons.append(
+            self.reasons.append(
                 f"INPUT SETTINGS --> KPOINTS or KSPACING: {cur_num_kpts} kpoints were "
                 f"used, but it should have been at least {valid_num_kpts}."
             )
 
+    def _check_kpoint_mesh_symmetry(self) -> None:
         # check for valid kpoint mesh (which depends on symmetry of the structure)
-        cur_kpoint_style = kpoints.get("generation_style").lower()
-        is_hexagonal = structure.lattice.is_hexagonal()
-        is_face_centered = structure.get_space_group_info()[0][0] == "F"
+
+        cur_kpoint_style = self.kpoints.get("generation_style").lower()
+        is_hexagonal = self.structure.lattice.is_hexagonal()
+        is_face_centered = self.structure.get_space_group_info()[0][0] == "F"
         monkhorst_mesh_is_invalid = is_hexagonal or is_face_centered
         if (
             cur_kpoint_style == "monkhorst"
             and monkhorst_mesh_is_invalid
-            and any(x % 2 == 0 for x in kpoints.get("kpoints")[0])
+            and any(x % 2 == 0 for x in self.kpoints.get("kpoints")[0])
         ):
             # only allow Monkhorst with all odd number of subdivisions per axis.
-            kx, ky, kz = kpoints.get("kpoints")[0]
-            reasons.append(
+            kx, ky, kz = self.kpoints.get("kpoints")[0]
+            self.reasons.append(
                 f"INPUT SETTINGS --> KPOINTS or KGAMMA: ({kx}x{ky}x{kz}) "
                 "Monkhorst-Pack kpoint mesh was used."
                 "To be compatible with the symmetry of the lattice, "
                 "a Monkhorst-Pack mesh should have only odd number of "
                 "subdivisions per axis."
             )
-
-        # Check for explicit kpoint meshes
-        if (not self.allow_explicit_kpoint_mesh) and len(kpoints["kpoints"]) > 1:
-            reasons.append(
-                "INPUT SETTINGS --> KPOINTS: explicitly defining "
-                "the k-point mesh is not currently allowed. "
-                "Automatic k-point generation is required."
-            )
-
-        # Check for user shifts
-        if (not self.allow_kpoint_shifts) and any(shift_val != 0 for shift_val in kpoints["usershift"]):
-            reasons.append("INPUT SETTINGS --> KPOINTS: shifting the kpoint mesh is not currently allowed.")
```

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_package_versions.py` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_package_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def package_version_check() -> None:
     """Warn the user if pymatgen / pymatgen-io-validation is not up-to-date."""
 
     packages = {
         "pymatgen": "Hence, if any pymatgen input sets have been updated, this validator will be outdated.",
-        "pymagen-io-validation": "Hence, if any checks in this package have been updated, the validator you use will be outdated.",
+        "pymatgen-io-validation": "Hence, if any checks in this package have been updated, the validator you use will be outdated.",
     }
 
     for package, context_msg in packages.items():
         if not is_package_is_up_to_date(package):
             warnings.warn(
                 "We *STRONGLY* recommend you to update your "
                 f"`{package}` package, which is behind the most "
```

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/check_potcar.py` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_potcar.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,112 +2,132 @@
 
 from __future__ import annotations
 from dataclasses import dataclass, field
 from importlib.resources import files as import_resource_files
 from monty.serialization import loadfn
 import numpy as np
 
+from pymatgen.io.validation.common import BaseValidator
+
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pymatgen.core import Structure
-    from pymatgen.io.vasp import Potcar
     from pymatgen.io.vasp.sets import VaspInputSet
 
 _potcar_summary_stats = loadfn(import_resource_files("pymatgen.io.vasp") / "potcar-summary-stats.json.bz2")
 
 
 @dataclass
-class CheckPotcar:
+class CheckPotcar(BaseValidator):
     """
     Check POTCAR against library of known valid POTCARs.
 
+    reasons : list[str]
+        A list of error strings to update if a check fails. These are higher
+        severity and would deprecate a calculation.
+    warnings : list[str]
+        A list of warning strings to update if a check fails. These are lower
+        severity and would flag a calculation for possible review.
+    valid_input_set: VaspInputSet
+        Valid input set to compare user INCAR parameters to.
+    structure: Pymatgen Structure
+        Structure used in the calculation.
+    potcar: dict
+        Spec (symbol, hash, and summary stats) for the POTCAR used in the calculation.
+    name : str = "Check POTCARs"
+        Name of the validator class
+    fast : bool = False
+        Whether to perform quick check.
+        True: stop validation if any check fails.
+        False: perform all checks.
     potcar_summary_stats : dict
         Dictionary of potcar summary data. Mapping is calculation type -> potcar symbol -> summary data.
-    data_match_tol : float
+    data_match_tol : float = 1.e-6
         Tolerance for matching POTCARs to summary statistics data.
+    fast : bool = False
+        True: stop validation when any single check fails
     """
 
+    reasons: list[str]
+    warnings: list[str]
+    valid_input_set: VaspInputSet = None
+    structure: Structure = None
+    potcars: dict = None
+    name: str = "Check POTCARs"
     potcar_summary_stats: dict = field(default_factory=lambda: _potcar_summary_stats)
     data_match_tol: float = 1.0e-6
+    fast: bool = False
 
-    def check(self, reasons: list[str], valid_input_set: VaspInputSet, structure: Structure, potcars: Potcar):
-        """
-        Checks to make sure the POTCAR is equivalent to the correct POTCAR from the pymatgen input set.
-
-        Parameters
-        -----------
-        reasons : list[str]
-            A list of error strings to update if a check fails. These are higher
-            severity and would deprecate a calculation.
-        valid_input_set: VaspInputSet
-            Valid input set to compare user INCAR parameters to.
-        structure: Pymatgen Structure
-            Structure used in the calculation.
-        potcar: Pymatgen Potcar
-            POTCAR used in the calculation.
+    def _check_potcar_spec(self):
         """
+        Checks to make sure the POTCAR is equivalent to the correct POTCAR from the pymatgen input set."""
 
         if not self.potcar_summary_stats:
+            # If no reference summary stats specified, or we're only doing a quick check,
+            # and there are already failure reasons, return
             return
 
-        if potcars is None:
-            reasons.append(
+        if self.potcars is None or any(potcar.get("summary_stats") is None for potcar in self.potcars):
+            self.reasons.append(
                 "PSEUDOPOTENTIALS --> Missing POTCAR files. "
                 "Alternatively, our potcar checker may have an issue--please create a GitHub issue if you "
                 "know your POTCAR exists and can be read by Pymatgen."
             )
             return
 
-        psp_subset = self.potcar_summary_stats.get(valid_input_set._config_dict["POTCAR_FUNCTIONAL"], {})
+        psp_subset = self.potcar_summary_stats.get(self.valid_input_set._config_dict["POTCAR_FUNCTIONAL"], {})
 
         valid_potcar_summary_stats = {}  # type: ignore
-        for element in structure.composition.remove_charges().as_dict():
-            potcar_symbol = valid_input_set._config_dict["POTCAR"][element]
+        for element in self.structure.composition.remove_charges().as_dict():
+            potcar_symbol = self.valid_input_set._config_dict["POTCAR"][element]
             for titel_no_spc in psp_subset:
                 for psp in psp_subset[titel_no_spc]:
                     if psp["symbol"] == potcar_symbol:
                         if titel_no_spc not in valid_potcar_summary_stats:
                             valid_potcar_summary_stats[titel_no_spc] = []
                         valid_potcar_summary_stats[titel_no_spc].append(psp)
 
         try:
             incorrect_potcars = []
-            for potcar in potcars:
+            for potcar in self.potcars:
                 reference_summary_stats = valid_potcar_summary_stats.get(potcar["titel"].replace(" ", ""), [])
 
                 if len(reference_summary_stats) == 0:
                     incorrect_potcars.append(potcar["titel"].split(" ")[1])
                     continue
 
                 for ref_psp in reference_summary_stats:
                     if found_match := self.compare_potcar_stats(ref_psp, potcar["summary_stats"]):
                         break
 
                 if not found_match:
                     incorrect_potcars.append(potcar["titel"].split(" ")[1])
+                    if self.fast:
+                        # quick return, only matters that one POTCAR didn't match
+                        break
 
             if len(incorrect_potcars) > 0:
                 # format error string
                 incorrect_potcars = [potcar.split("_")[0] for potcar in incorrect_potcars]
                 if len(incorrect_potcars) == 2:
                     incorrect_potcars = ", ".join(incorrect_potcars[:-1]) + f" and {incorrect_potcars[-1]}"  # type: ignore
                 elif len(incorrect_potcars) >= 3:
                     incorrect_potcars = ", ".join(incorrect_potcars[:-1]) + "," + f" and {incorrect_potcars[-1]}"  # type: ignore
 
-                reasons.append(
+                self.reasons.append(
                     f"PSEUDOPOTENTIALS --> Incorrect POTCAR files were used for {incorrect_potcars}. "
                     "Alternatively, our potcar checker may have an issue--please create a GitHub issue if you "
                     "believe the POTCARs used are correct."
                 )
 
         except KeyError as e:
             print(f"POTCAR check exception: {e}")
             # Assume it is an old calculation without potcar_spec data and treat it as failing the POTCAR check
-            reasons.append(
+            self.reasons.append(
                 "Issue validating POTCARS --> Likely due to an old version of Emmet "
                 "(wherein potcar summary_stats is not saved in TaskDoc), though "
                 "other errors have been seen. Hence, it is marked as invalid."
             )
 
     def compare_potcar_stats(self, potcar_stats_1: dict, potcar_stats_2: dict) -> bool:
         """Utility function to compare PotcarSingle._summary_stats."""
```

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/compare_to_MP_ehull.py` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/compare_to_MP_ehull.py`

 * *Files identical despite different names*

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/settings.py` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 class IOValidationSettings(BaseSettings):
     """
     Settings for pymatgen-io-validation
     """
 
     config_file: str = Field(DEFAULT_CONFIG_FILE_PATH, description="File to load alternative defaults from")
 
+    CHECK_PYPI_AT_LOAD: bool = Field(
+        False,
+        description=(
+            "Whether to do a version check when this module is loaded. "
+            "Helps user ensure most recent parameter checks are used."
+        ),
+    )
+
     VASP_KPTS_TOLERANCE: float = Field(
         0.9,
         description="Relative tolerance for kpt density to still be a valid task document",
     )
 
     VASP_ALLOW_KPT_SHIFT: bool = Field(
         False,
@@ -88,14 +96,22 @@
     VASP_DEFAULTS_FILENAME: Union[str, Path] = Field(
         default=import_resource_files("pymatgen.io.validation") / "vasp_defaults.yaml",
         description="Path to the  of the YAML file containing default values of VASP parameters.",
     )
 
     model_config = SettingsConfigDict(env_prefix="pymatgen_io_validation_", extra="ignore")
 
+    FAST_VALIDATION: bool = Field(
+        default=False,
+        description=(
+            "Whether to attempt to find all reasons a calculation fails (False), "
+            "or stop validation if any single check fails."
+        ),
+    )
+
     @model_validator(mode="before")
     @classmethod
     def load_default_settings(cls, values):
         """
         Loads settings from a root file if available and uses that as defaults in
         place of built in defaults
         """
```

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/validation.py` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 # TODO: MK: because more kpoints are needed for metals given the more complicated Fermi surfaces, and MPMetalRelaxSet uses more kpoints
 from pymatgen.io.vasp.sets import MPMetalRelaxSet
 
 from emmet.core.tasks import TaskDoc
 from emmet.core.vasp.task_valid import TaskDocument
 from emmet.core.base import EmmetBaseModel
 from emmet.core.mpid import MPID
+from emmet.core.utils import jsanitize
 from emmet.core.vasp.calc_types.enums import CalcType, TaskType
 from emmet.core.vasp.calc_types import (
     RunType,
     calc_type as emmet_calc_type,
     run_type as emmet_run_type,
     task_type as emmet_task_type,
 )
+from pymatgen.core import Structure
 from pymatgen.io.validation.check_incar import CheckIncar
 from pymatgen.io.validation.check_common_errors import (
     CheckCommonErrors,
     CheckVaspVersion,
 )
 from pymatgen.io.validation.check_kpoints_kspacing import CheckKpointsKspacing
 from pymatgen.io.validation.check_potcar import CheckPotcar
@@ -55,22 +57,14 @@
 
     valid: bool = Field(False, description="Whether this task is valid or not")
 
     last_updated: datetime = Field(
         description="Last updated date for this document",
         default_factory=datetime.utcnow,
     )
-    check_package_versions: bool = Field(
-        False,
-        description=(
-            "Whether to check if the currently installed versions "
-            "of pymatgen and pymatgen-io-validation are the most "
-            "up to date versions on PyPI."
-        ),
-    )
 
     reasons: list[str] = Field(None, description="List of deprecation tags detailing why this task isn't valid")
 
     warnings: list[str] = Field([], description="List of potential warnings about this calculation")
 
     # data: Dict = Field(
     #     description="Dictionary of data used to perform validation."
@@ -82,187 +76,206 @@
         Optionally check whether package versions are up to date with PyPI.
 
         Parameters
         -----------
         context : .Any
             Has no effect at present, kept to retain structure of pydantic .BaseModel
         """
-        if self.check_package_versions:
-            from check_package_versions import package_version_check
 
-            package_version_check()
+        self.valid = len(self.reasons) == 0
 
     class Config:  # noqa
         extra = "allow"
 
     @classmethod
-    def from_task_doc(
+    def from_task_doc(cls, task_doc: TaskDoc | TaskDocument, **kwargs) -> ValidationDoc:
+        """
+        Determines if a calculation is valid based on expected input parameters from a pymatgen inputset
+
+        Args:
+            task_doc: the task document to process
+        Possible kwargs for `from_dict` method:
+            input_sets: a dictionary of task_types -> pymatgen input set for validation
+            potcar_summary_stats: Dictionary of potcar summary data. Mapping is calculation type -> potcar symbol -> summary data.
+            kpts_tolerance: the tolerance to allow kpts to lag behind the input set settings
+            allow_kpoint_shifts: Whether to consider a task valid if kpoints are shifted by the user
+            allow_explicit_kpoint_mesh: Whether to consider a task valid if the user defines an explicit kpoint mesh
+            fft_grid_tolerance: Relative tolerance for FFT grid parameters to still be a valid
+            num_ionic_steps_to_avg_drift_over: Number of ionic steps to average over when validating drift forces
+            max_allowed_scf_gradient: maximum uphill gradient allowed for SCF steps after the
+                initial equillibriation period. Note this is in eV per atom.
+            fast : whether to stop validation when any check fails
+        """
+
+        if isinstance(task_doc, TaskDocument):
+            task_doc = TaskDoc(**task_doc.model_dump())
+
+        return cls.from_dict(jsanitize(task_doc), **kwargs)
+
+    @classmethod
+    def from_dict(
         cls,
-        task_doc: TaskDoc | TaskDocument,
+        task_doc: dict,
         input_sets: dict[str, ImportString] = SETTINGS.VASP_DEFAULT_INPUT_SETS,
         check_potcar: bool = True,
         kpts_tolerance: float = SETTINGS.VASP_KPTS_TOLERANCE,
         allow_kpoint_shifts: bool = SETTINGS.VASP_ALLOW_KPT_SHIFT,
         allow_explicit_kpoint_mesh: str | bool = SETTINGS.VASP_ALLOW_EXPLICIT_KPT_MESH,
         fft_grid_tolerance: float = SETTINGS.VASP_FFT_GRID_TOLERANCE,
         num_ionic_steps_to_avg_drift_over: int = SETTINGS.VASP_NUM_IONIC_STEPS_FOR_DRIFT,
         max_allowed_scf_gradient: float = SETTINGS.VASP_MAX_SCF_GRADIENT,
+        fast: bool = SETTINGS.FAST_VALIDATION,
     ) -> ValidationDoc:
         """
         Determines if a calculation is valid based on expected input parameters from a pymatgen inputset
 
         Args:
             task_doc: the task document to process
+        Kwargs:
             input_sets: a dictionary of task_types -> pymatgen input set for validation
             potcar_summary_stats: Dictionary of potcar summary data. Mapping is calculation type -> potcar symbol -> summary data.
             kpts_tolerance: the tolerance to allow kpts to lag behind the input set settings
             allow_kpoint_shifts: Whether to consider a task valid if kpoints are shifted by the user
             allow_explicit_kpoint_mesh: Whether to consider a task valid if the user defines an explicit kpoint mesh
             fft_grid_tolerance: Relative tolerance for FFT grid parameters to still be a valid
             num_ionic_steps_to_avg_drift_over: Number of ionic steps to average over when validating drift forces
             max_allowed_scf_gradient: maximum uphill gradient allowed for SCF steps after the
                 initial equillibriation period. Note this is in eV per atom.
+            fast : whether to stop validation when any check fails
         """
 
-        if isinstance(task_doc, TaskDocument):
-            task_doc = TaskDoc(**task_doc.model_dump())
+        bandgap = task_doc["output"]["bandgap"]
+        calcs_reversed = task_doc["calcs_reversed"]
 
-        bandgap = task_doc.output.bandgap
-        calcs_reversed = task_doc.calcs_reversed
-        calcs_reversed = [
-            calc.model_dump() for calc in calcs_reversed
-        ]  # convert to dictionary to use built-in `.get()` method
-
-        parameters = (
-            task_doc.input.parameters
-        )  # used for most input tag checks (as this is more reliable than examining the INCAR file directly in most cases)
-        incar = calcs_reversed[0]["input"][
-            "incar"
-        ]  # used for INCAR tag checks where you need to look at the actual INCAR (semi-rare)
-        if task_doc.orig_inputs is None:
-            orig_inputs = {}
-        else:
-            orig_inputs = task_doc.orig_inputs.model_dump()
-            if orig_inputs["kpoints"] is not None:
-                orig_inputs["kpoints"] = orig_inputs["kpoints"].as_dict()
-
-        potcars = calcs_reversed[0]["input"]["potcar_spec"]
-
-        calc_type = _get_calc_type(calcs_reversed, orig_inputs)
-        task_type = _get_task_type(calcs_reversed, orig_inputs)
-        run_type = _get_run_type(calcs_reversed)
+        # used for most input tag checks (as this is more reliable than examining the INCAR file directly in most cases)
+        parameters = task_doc["input"]["parameters"]
 
-        if allow_explicit_kpoint_mesh == "auto":
-            if "NSCF" in calc_type.name:
-                allow_explicit_kpoint_mesh = True
-            else:
-                allow_explicit_kpoint_mesh = False
+        # used for INCAR tag checks where you need to look at the actual INCAR (semi-rare)
+        incar = calcs_reversed[0]["input"]["incar"]
 
-        # Why was this lingering here?
-        # task_doc.chemsys
+        orig_inputs = {} if (task_doc["orig_inputs"] is None) else task_doc["orig_inputs"]
+
+        cls_kwargs: dict[str, Any] = {
+            "task_id": (
+                task_doc["task_id"] if task_doc["task_id"] else -1
+            ),  # Unsure about what might be a better way to do this...
+            "calc_type": _get_calc_type(calcs_reversed, orig_inputs),
+            "task_type": _get_task_type(calcs_reversed, orig_inputs),
+            "run_type": _get_run_type(calcs_reversed),
+            "reasons": [],
+            "warnings": [],
+        }
 
         vasp_version = [int(x) for x in calcs_reversed[0]["vasp_version"].split(".")[:3]]
+        CheckVaspVersion(
+            reasons=cls_kwargs["reasons"],
+            warnings=cls_kwargs["warnings"],
+            vasp_version=vasp_version,
+            parameters=parameters,
+            incar=incar,
+            defaults=_vasp_defaults,
+            fast=fast,
+        ).check()
+
+        if len(cls_kwargs["reasons"]) > 0 and fast:
+            return cls(**cls_kwargs)
+
+        if allow_explicit_kpoint_mesh == "auto":
+            allow_explicit_kpoint_mesh = True if "NSCF" in cls_kwargs["calc_type"].name else False
 
         if calcs_reversed[0].get("input", {}).get("structure", None):
             structure = calcs_reversed[0]["input"]["structure"]
         else:
-            structure = task_doc.input.structure or task_doc.output.structure
-
-        reasons = []
-        # data = {}  # type: ignore
-        warnings: list[str] = []
-
-        if f"{run_type}".upper() not in {"GGA", "GGA+U", "PBE", "PBE+U", "R2SCAN"}:
-            reasons.append(f"FUNCTIONAL --> Functional {run_type} not currently accepted.")
+            structure = task_doc["input"]["structure"] or task_doc["output"]["structure"]
+        structure = Structure.from_dict(structure)
 
         try:
-            valid_input_set = _get_input_set(run_type, task_type, calc_type, structure, input_sets, bandgap)
+            valid_input_set = _get_input_set(
+                cls_kwargs["run_type"], cls_kwargs["task_type"], cls_kwargs["calc_type"], structure, input_sets, bandgap
+            )
         except Exception as e:
-            reasons.append(
+            cls_kwargs["reasons"].append(
                 "NO MATCHING MP INPUT SET --> no matching MP input set was found. If you believe this to be a mistake, please create a GitHub issue."
             )
             valid_input_set = None
             print(f"Error while finding MP input set: {e}.")
 
-        if parameters == {} or parameters is None:
-            reasons.append(
-                "CAN NOT PROPERLY PARSE CALCULATION --> Issue parsing input parameters from the vasprun.xml file."
-            )
-        elif valid_input_set:
-            # Get subset of POTCAR summary stats to validate calculation
+        if valid_input_set:
 
-            if check_potcar:
-                CheckPotcar().check(
-                    reasons=reasons, valid_input_set=valid_input_set, structure=structure, potcars=potcars
-                )
+            # Tests ordered by expected computational burden - help optimize `fast` check
+            # Intuitively, more important checks (INCAR, KPOINTS, and POTCAR settings) would come first
+            # But to optimize speed in fast mode (relevant for validating a large batch of calculations)
+            # the faster checks have to come first:
+            #   1. VASP version
+            #   2. Common errors (known bugs in VASP, erratic SCF convergence, etc.)
+            #   3. KPOINTS or KSPACING (from INCAR)
+            #   4. INCAR (many sequential checks of possible INCAR tags + updating defaults)
 
             # TODO: check for surface/slab calculations!!!!!!
 
-            CheckVaspVersion(defaults=_vasp_defaults).check(reasons, vasp_version, parameters, incar)
-
             CheckCommonErrors(
+                reasons=cls_kwargs["reasons"],
+                warnings=cls_kwargs["warnings"],
+                task_doc=task_doc,
+                parameters=parameters,
+                structure=structure,
+                run_type=cls_kwargs["run_type"],
+                fast=fast,
                 defaults=_vasp_defaults,
                 valid_max_allowed_scf_gradient=max_allowed_scf_gradient,
                 num_ionic_steps_to_avg_drift_over=num_ionic_steps_to_avg_drift_over,
-            ).check(reasons=reasons, warnings=warnings, task_doc=task_doc, parameters=parameters, structure=structure)
+            ).check()
 
             CheckKpointsKspacing(
+                reasons=cls_kwargs["reasons"],
+                warnings=cls_kwargs["warnings"],
+                valid_input_set=valid_input_set,
+                kpoints=calcs_reversed[0]["input"]["kpoints"],
+                structure=structure,
                 defaults=_vasp_defaults,
                 kpts_tolerance=kpts_tolerance,
                 allow_explicit_kpoint_mesh=allow_explicit_kpoint_mesh,
                 allow_kpoint_shifts=allow_kpoint_shifts,
-            ).check(
-                reasons=reasons,
-                valid_input_set=valid_input_set,
-                kpoints=calcs_reversed[0]["input"]["kpoints"],
-                structure=structure,
-            )
+                fast=fast,
+            ).check()
 
-            CheckIncar(defaults=_vasp_defaults, fft_grid_tolerance=fft_grid_tolerance).check(
-                reasons=reasons,
-                warnings=warnings,
+            if check_potcar:
+                CheckPotcar(
+                    reasons=cls_kwargs["reasons"],
+                    warnings=cls_kwargs["warnings"],
+                    valid_input_set=valid_input_set,
+                    structure=structure,
+                    potcars=calcs_reversed[0]["input"]["potcar_spec"],
+                    fast=fast,
+                ).check()
+
+            CheckIncar(
+                reasons=cls_kwargs["reasons"],
+                warnings=cls_kwargs["warnings"],
                 valid_input_set=valid_input_set,
                 task_doc=task_doc,
                 parameters=parameters,
                 structure=structure,
                 vasp_version=vasp_version,
-                task_type=task_type,
-            )
-
-        # Unsure about what might be a better way to do this...
-        task_id = task_doc.task_id if task_doc.task_id else -1
+                task_type=cls_kwargs["task_type"],
+                defaults=_vasp_defaults,
+                fft_grid_tolerance=fft_grid_tolerance,
+                fast=fast,
+            ).check()
 
-        return cls(
-            task_id=task_id,
-            calc_type=calc_type,
-            run_type=run_type,
-            task_type=task_type,
-            valid=len(reasons) == 0,
-            reasons=reasons,
-            warnings=warnings,
-        )
+        return cls(**cls_kwargs)
 
     @classmethod
-    def from_directory(
-        cls,
-        dir_name: Path | str,
-        input_sets: dict[str, ImportString] = SETTINGS.VASP_DEFAULT_INPUT_SETS,
-        check_potcar: bool = True,
-        kpts_tolerance: float = SETTINGS.VASP_KPTS_TOLERANCE,
-        allow_kpoint_shifts: bool = SETTINGS.VASP_ALLOW_KPT_SHIFT,
-        allow_explicit_kpoint_mesh: str | bool = SETTINGS.VASP_ALLOW_EXPLICIT_KPT_MESH,
-        fft_grid_tolerance: float = SETTINGS.VASP_FFT_GRID_TOLERANCE,
-        num_ionic_steps_to_avg_drift_over: int = SETTINGS.VASP_NUM_IONIC_STEPS_FOR_DRIFT,
-        max_allowed_scf_gradient: float = SETTINGS.VASP_MAX_SCF_GRADIENT,
-    ) -> ValidationDoc:
+    def from_directory(cls, dir_name: Path | str, **kwargs) -> ValidationDoc:
         """
         Determines if a calculation is valid based on expected input parameters from a pymatgen inputset
 
         Args:
             dir_name: the directory containing the calculation files to process
+        Possible kwargs for `from_dict` method:
             input_sets: a dictionary of task_types -> pymatgen input set for validation
             check_potcar: Whether to check POTCARs against known libraries.
             kpts_tolerance: the tolerance to allow kpts to lag behind the input set settings
             allow_kpoint_shifts: Whether to consider a task valid if kpoints are shifted by the user
             allow_explicit_kpoint_mesh: Whether to consider a task valid if the user defines an explicit kpoint mesh
             fft_grid_tolerance: Relative tolerance for FFT grid parameters to still be a valid
             num_ionic_steps_to_avg_drift_over: Number of ionic steps to average over when validating drift forces
@@ -271,29 +284,17 @@
         """
         try:
             task_doc = TaskDoc.from_directory(
                 dir_name=dir_name,
                 volumetric_files=(),
             )
 
-            validation_doc = ValidationDoc.from_task_doc(
-                task_doc=task_doc,
-                input_sets=input_sets,
-                check_potcar=check_potcar,
-                kpts_tolerance=kpts_tolerance,
-                allow_kpoint_shifts=allow_kpoint_shifts,
-                allow_explicit_kpoint_mesh=allow_explicit_kpoint_mesh,
-                fft_grid_tolerance=fft_grid_tolerance,
-                num_ionic_steps_to_avg_drift_over=num_ionic_steps_to_avg_drift_over,
-                max_allowed_scf_gradient=max_allowed_scf_gradient,
-            )
+            return cls.from_task_doc(task_doc=task_doc, **kwargs)
 
-            return validation_doc
         except Exception as e:
-            print(e)
             if "no vasp files found" in str(e).lower():
                 raise Exception(f"NO CALCULATION FOUND --> {dir_name} is not a VASP calculation directory.")
             else:
                 raise Exception(
                     f"CANNOT PARSE CALCULATION --> Issue parsing results. This often means your calculation did not complete. The error stack reads: \n {e}"
                 )
```

### Comparing `pymatgen-io-validation-0.0.1/pymatgen/io/validation/vasp_defaults.yaml` & `pymatgen_io_validation-0.0.2/pymatgen/io/validation/vasp_defaults.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-io-validation-0.0.1/pymatgen_io_validation.egg-info/PKG-INFO` & `pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,137 +1,157 @@
 Metadata-Version: 2.1
 Name: pymatgen-io-validation
-Version: 0.0.1
+Version: 0.0.2
 Summary: A comprehensive I/O validator for electronic structure calculations
-Home-page: https://github.com/matthewkuner/pymatgen-io-validation
-Author: Matthew Kuner, Janosh Riebesell, Jason Munro, Aaron Kaplan
-Author-email: matthewkuner@berkeley.edu
+Home-page: https://github.com/materialsproject/pymatgen-io-validation
+Author: Janosh Riebesell, Jason Munro, Aaron Kaplan
+Author-email: Matthew Kuner <matthewkuner@gmail.com>
 Maintainer: Matthew Kuner
-License: BSD
-Description: pymatgen-io-validation
-        =====
-        
-        This package is an extension to `pymatgen` for performing I/O validation. Specifically, this package checks for discrepancies between a specific calculation and a provided input set; it also checks for known bugs when certain input parameters are used in combination, alongside several other small checks. The initial motivation for creating this package was to validate VASP calculations performed by groups outside of the Materials Project (MP), enabling their raw data to be included in the MP Database.
-        
-        
-        Usage
-        =====
-        
-        For validating calculations from the raw files, run:
-        ```
-        from pymatgen.io.validation import ValidationDoc
-        validation_doc = ValidationDoc.from_directory(dir_name = path_to_vasp_calculation_directory)
-        ```
-        
-        In the above case, whether a calculation passes the validator can be accessed via `validation_doc.valid`. Moreover, reasons for an invalidated calculation can be accessed via `validation_doc.reasons` (this will be empty for valid calculations). Last but not least, warnings for potential issues (sometimes minor, sometimes major) can be accessed via `validation_doc.warnings`.
-        \
-        \
-        For validating calculations from `TaskDoc` objects from the [Emmet](https://github.com/materialsproject/emmet) package, run:
-        ```
-        from pymatgen.io.validation import ValidationDoc
-        validation_doc = ValidationDoc.from_task_doc(task_doc = my_task_doc)
-        ```
-        
-        Contributors
-        =====
-        
-        * [Matthew Kuner](https://github.com/matthewkuner) (lead), email: matthewkuner@gmail.com
-        * [Aaron Kaplan](https://github.com/esoteric-ephemera)
-        * [Janosh Riebesell](https://github.com/janosh)
-        * [Jason Munro](https://github.com/munrojm)
-        
-        
-        Rationale
-        ====
-        
-        | **Parameter** | **Reason** |
-        | ---- | ---- |
-        | ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states “please do not use this tag [ADDGRID] as default in all your calculations!”. ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
-        | AEXX / AMGGAX / AMGGAC / AGGAX / ALDAC / ALDAX | These parameters should be the VASP defaults unless otherwise specified in a given MP input set, as changing them is effectively a change to the level of theory. |
-        | ALGO / IALGO | ALGO must be one of: "Normal", "Conjugate", "All", "Fast", "Exact". (This corresponds to an IALGO of 38, 58, 58, 68, 90, respectively). |
-        | DEPER / EBREAK / WEIMIN | DEPER, EBREAK, and WEIMIN should not be changed according to the VASP wiki, hence MP requires them to remain as their default values. |
-        | EDIFF | EDIFF must be equal to or greater than the value in the relevant MP input set. This will ensure compatibility between results with those in the MP Database. |
-        | EDIFFG | Should be the same or better than in the relevant MP input set. For MP input sets with an energy-based cutoff, the calculation must have an energy change between the last two steps be less in magnitude than the specified EDIFFG (so even if your calculation uses force-based convergence, the energy must converge within the MP input set’s specification). The same logic applies to MP input sets with force-based EDIFFG settings. |
-        | EFERMI | EFERMI must be one of: "LEGACY", "MIDGAP" |
-        | EFIELD | Current MP input sets used to construct the main MP database do not set EFIELD, and hence we require this to be unset or set to 0. |
-        | ENAUG | If ENAUG is present in the relevant MP input set, then a calculation’s ENAUG must be equal to or better than that value. |
-        | ENCUT | ENCUT must be equal to or greater than the value in the relevant MP input set, as otherwise results will likely be incompatible with MP. |
-        | ENINI | ENINI must not be adjusted for high-throughput calculations, and hence should be left equal to the value used for ENCUT in the relevant MP input set. Values greater than the ENCUT in the relevant MP input set will also be accepted, though we expect this to be uncommon and do not recommend it. |
-        | EPSILON | EPSILON must be set to the VASP default of 1. Changing the dielectric constant of the medium will cause results to be incompatible with MP. |
-        | GGA / METAGGA | The level of theory used must match the relevant MP input set. Moreover, GGA and METAGGA should never be set simultaneously, as this has been shown to result in seriously erroneous results. See https://github.com/materialsproject/atomate2/issues/453#issuecomment-1699605867 for more details. |
-        | GGA_COMPAT | GGA_COMPAT must be set to the VASP default of True. The VASP manual only recommends setting this to False for noncollinear magnetic calculations, which are not currently included in the MP database. |
-        | IBRION | IBRION values must be one of: -1, 1, 2. Other IBRION values correspond to non-standard forms of DFT calculations that are not included in the MP database. (Note that, while phonon data is included in the MP database, such values are not calculated using, say, IBRION = 5. Such logic applies to all other IBRION values not allowed). |
-        | ICHARG | ICHARG must be set to be compatible with the calculation type. For example, if the relevant MP input set is for a SCF calculation, ICHARG $\leq 9$ must be used. For NSCF calculations, the value for ICHARG must exactly match the value contained in the relevant MP input set. |
-        | ICORELEVEL | ICORELEVEL must be set to 0. MP does not explicitly calculate core energies. |
-        | IDIPOL | IDIPOL must be set to 0 (the VASP default). |
-        | IMAGES | IMAGES must be set to 0 to match MP calculations. |
-        | INIWAV | INIWAV must be set as the VASP default of 1 to be consistent with MP calculations. |
-        | ISPIN | All values of ISPIN are allowed, though it should be noted that virtually all MP calculations permit spin symmetry breaking, and have ferromagnetic, antiferrogmanetic, or nonmagnetic ordering. |
-        | ISMEAR | The appropriate ISMEAR depends on the bandgap of the material (which cannot be known a priori). As per the VASP manual: for metals (bandgap = 0), any ISMEAR value in [0, 1, 2] is acceptable. For nonmetals (bandgap > 0), any ISMEAR value in [-5, 0] is acceptable. Hence, for those who are performing normal relaxations/static calculations and want to ensure their calculations are MP-compatible, we recommend setting ISMEAR to 0. |
-        | ISIF | MP allows any ISIF $\geq 2$. This value is restricted as such simply because all ISIF values $\geq 2$ output the complete stress tensor. |
-        | ISYM | ISYM must be one of -1, 0, 1, 2, except for when the relevant MP input set uses a hybrid functional, in which case ISYM=3 is also allowed. |
-        | ISTART | ISTART must be one of: 0, 1, 2. |
-        | IVDW | IVDW must be set to 0. MP currently does not apply any vdW dispersion corrections. |
-        | IWAVPR | IWAVPR must be set to 0 (the default). VASP discourages users from setting this tag. |
-        | KGAMMA | KGAMMA must be set to True (the VASP default). This is only relevant when no KPOINTS file is used. |
-        | KSPACING / KPOINTS | The KSPACING parameter or KPOINTS file must correspond with at least 0.9 times **the number of KPOINTS in the non-symmetry-reduced Brillouin zone specified by the relevant MP input set** (i.e., not the number of points in the irreducible wedge of the first Brillouin zone). Hence, either method of specifying the KPOINTS can be chosen. This ensures that a calculation uses a comparable number of kpoints to MP. |
-        | Kpoint mesh type (for KPOINTS) | The type of Kpoint mesh must be valid for the symmetry of the crystal structure in the calculation. For example, for a hexagonal closed packed structure, one must use a $\Gamma$-centered mesh. All Kpoints generated using Pymatgen *should* be valid. |
-        | LASPH | LASPH must be set to True (this is **<u>*not*</u>** the VASP default). |
-        | LCALCEPS | LCALCEPS must be set to False (the VASP default). |
-        | LBERRY | LBERRY must be set to False (the VASP default). |
-        | LCALCPOL | LCALCPOL  must be set to False (the VASP default). |
-        | LCHIMAG | LCHIMAG must be set to False (the VASP default). |
-        | LCORR | LCORR must be set to True (the VASP default) for calculations with IALGO = 58. |
-        | LDAU / LDAUU / LDAUJ / LDAUL / LDAUTYPE | For DFT$`+U`$ calculations, all parameters corresponding to $+U$ or $+J$ corrections must exactly match those specified in the relevant MP input set. Alternatively, LDAU = False (DFT) is always acceptable. |
-        | LDIPOL | LDIPOL must be set to False (the VASP default). |
-        | LMONO | LMONO must be set to False (the VASP default). |
-        | LEFG | LEFG must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
-        | LEPSILON | LEPSILON must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
-        | LHFCALC | The value of LHFCALC should match that of the relevant MP input set, as it will otherwise result in a change in the level of theory applied in the calculation. |
-        | LHYPERFINE | LHYPERFINE must be set to False (the VASP default). |
-        | LKPROJ | LKPROJ must be set to False (the VASP default). |
-        | LKPOINTS_OPT | LKPOINTS_OPT must be set to False. |
-        | LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that “Energies should be evaluated with the default setting for LMAXPAW”. |
-        | LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the “bench_vasp_pars.docx” document in https://github.com/materialsproject/pymatgen/issues/3322. |
-        | LMAXTAU | LMAXTAU must be set to 6 (the VASP default when using LASPH = True). |
-        | LMP2LT / LSMP2LT | Both must be set to False (VASP defaults) |
-        | LNONCOLLINEAR / LSORBIT | Both must be set to False (VASP defaults) |
-        | LOCPROJ | LOCPROJ must be set to None (the VASP default). |
-        | LOPTICS | LOPTICS must be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
-        | LORBIT | LORBIT must **<u>*not*</u>** be None if the user also sets ISPIN=2, otherwise all values of LORBIT are acceptable. This is due to magnetization values not being output when ISPIN=2 and LORBIT = None are set together. |
-        | LREAL | If the LREAL in the relevant MP input set is “Auto”, then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
-        | LRPA | LRPA must be set to False (the VASP default). MP does not currently support random phase approximation (RPA) calculations. |
-        | LSPECTRAL | LSPECTRAL must be set to False (the VASP default for most calculations). |
-        | LSUBROT | LSUBROT must be set to False (the VASP default). |
-        | MAGMOM | While any initial magnetic moments are allowed, the final total magnetic moment for any given atom must be less than 5 $\mu_B$ (Bohr magnetons) (except for elements Gd and Eu, which must be less than 10 $\mu_B$). This simply serves as a filter for erroneous data. |
-        | ML_LMFF | ML_LMFF must be set to False (the VASP default). |
-        | NGX / NGY / NGZ | The values for NGX/NGY/NGZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
-        | NGFX / NGFY / NGFZ | The values for NGFX/NGFY/NGFZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
-        | NLSPLINE | NLSPLINE should be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
-        | NBANDS | NBANDS must be greater than the value $\mathrm{ceil}(\mathrm{NELECT}/2) + 1 $(minimum allowable number of bands to avoid degeneracy) and less than 4 times (minimum allowable number of bands to avoid degeneracy). For high-throughput calculations, it is generally recommended to not set this parameter directly. See https://github.com/materialsproject/custodian/issues/224 for more information. |
-        | NELECT | NELECT must not be changed from the default value VASP would use for the particular structure and pseudopotentials calculated. The easiest way to ensure that NELECT is compliant with MP data is to simply not specify NELECT in the INCAR file. |
-        | NWRITE | NWRITE must be set to be $\geq 2$ (the VASP default is 2). |
-        | POTIM | POTIM $\leq 5$. We suggest not setting POTIM in the INCAR file, and rather allowing VASP to set it to the default value of 0.5. |
-        | PSTRESS | PSTRESS must be set to exactly 0.0 (the VASP default). |
-        | PREC | PREC must be one of: "High", "Accurate". |
-        | ROPT | ROPT should be set to be less than or equal to the default ROPT value (which is set based on the PREC tag). Hence, it is recommended to not set the ROPT tag in the INCAR file. |
-        | RWIGS | RWIGS should not be set in the INCAR file. |
-        | SCALEE | SCALEE should not be set in the INCAR file. |
-        | SYMPREC | SYMPREC must be less than or equal to 1e-3 (as this is the maximum value that the Custodian package will set SYMPREC as of March 2024). For general use, we recommend leaving SYMPREC as the default generated by your desired MP input set. |
-        | SIGMA | There are several rules for setting SIGMA:  <ol> <li> SIGMA  must be $\leq 0.05$ for non-metals (bandgap $>  0$). </li> <li> SIGMA must be $\leq 0.2$ for a metal (bandgap = 0). </li> <li> For metals, the SIGMA value must be small enough that the entropy term in the energy is $\leq$ 1 meV/atom (as suggested by the VASP manual). </li> </ol> |
-        | VCA | MP data does not include Virtual Crystal Approximation (VCA) calculations from VASP. As such, this parameter should not be set. |
-        | VASP version | The following versions of VASP are allowed: 5.4.4 or $>$ 6.0.0. For example, versions $<=$ 5.4.3 are not allowed, whereas version 6.3.1 is allowed. |
-        
-Keywords: pymatgen
-Platform: UNKNOWN
+License: modified BSD
+Keywords: io,validation,dft,vasp
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pymatgen
+Requires-Dist: numpy
+Requires-Dist: requests
+Provides-Extra: dev
+Requires-Dist: pre-commit>=2.12.1; extra == "dev"
+Provides-Extra: tests
+Requires-Dist: pytest==8.0.2; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0; extra == "tests"
+Requires-Dist: types-requests; extra == "tests"
+
+pymatgen-io-validation
+=====
+
+This package is an extension to `pymatgen` for performing I/O validation. Specifically, this package checks for discrepancies between a specific calculation and a provided input set; it also checks for known bugs when certain input parameters are used in combination, alongside several other small checks. The motivation for creating this package was to ensure VASP calculations performed by groups outside of the Materials Project (MP) are compliant with MP data, thus enabling their raw data to be included in the MP Database.
+
+
+Installation
+=====
+
+You can install this package by simply running
+
+`pip install pymatgen-io-validation`
+
+
+Usage
+=====
+
+For validating calculations from the raw files, run:
+```
+from pymatgen.io.validation import ValidationDoc
+validation_doc = ValidationDoc.from_directory(dir_name = path_to_vasp_calculation_directory)
+```
+
+In the above case, whether a calculation passes the validator can be accessed via `validation_doc.valid`. Moreover, reasons for an invalidated calculation can be accessed via `validation_doc.reasons` (this will be empty for valid calculations). Last but not least, warnings for potential issues (sometimes minor, sometimes major) can be accessed via `validation_doc.warnings`.
+\
+\
+For validating calculations from `TaskDoc` objects from the [Emmet](https://github.com/materialsproject/emmet) package, run:
+```
+from pymatgen.io.validation import ValidationDoc
+validation_doc = ValidationDoc.from_task_doc(task_doc = my_task_doc)
+```
+
+Contributors
+=====
+
+* [Matthew Kuner](https://github.com/matthewkuner) (lead), email: matthewkuner@gmail.com
+* [Aaron Kaplan](https://github.com/esoteric-ephemera)
+* [Janosh Riebesell](https://github.com/janosh)
+* [Jason Munro](https://github.com/munrojm)
+
+
+Rationale
+====
+
+| **Parameter** | **Reason** |
+| ---- | ---- |
+| ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states “please do not use this tag [ADDGRID] as default in all your calculations!”. ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
+| AEXX / AMGGAX / AMGGAC / AGGAX / ALDAC / ALDAX | These parameters should be the VASP defaults unless otherwise specified in a given MP input set, as changing them is effectively a change to the level of theory. |
+| ALGO / IALGO | ALGO must be one of: "Normal", "Conjugate", "All", "Fast", "Exact". (This corresponds to an IALGO of 38, 58, 58, 68, 90, respectively). |
+| DEPER / EBREAK / WEIMIN | DEPER, EBREAK, and WEIMIN should not be changed according to the VASP wiki, hence MP requires them to remain as their default values. |
+| EDIFF | EDIFF must be equal to or greater than the value in the relevant MP input set. This will ensure compatibility between results with those in the MP Database. |
+| EDIFFG | Should be the same or better than in the relevant MP input set. For MP input sets with an energy-based cutoff, the calculation must have an energy change between the last two steps be less in magnitude than the specified EDIFFG (so even if your calculation uses force-based convergence, the energy must converge within the MP input set’s specification). The same logic applies to MP input sets with force-based EDIFFG settings. |
+| EFERMI | EFERMI must be one of: "LEGACY", "MIDGAP" |
+| EFIELD | Current MP input sets used to construct the main MP database do not set EFIELD, and hence we require this to be unset or set to 0. |
+| ENAUG | If ENAUG is present in the relevant MP input set, then a calculation’s ENAUG must be equal to or better than that value. |
+| ENCUT | ENCUT must be equal to or greater than the value in the relevant MP input set, as otherwise results will likely be incompatible with MP. |
+| ENINI | ENINI must not be adjusted for high-throughput calculations, and hence should be left equal to the value used for ENCUT in the relevant MP input set. Values greater than the ENCUT in the relevant MP input set will also be accepted, though we expect this to be uncommon and do not recommend it. |
+| EPSILON | EPSILON must be set to the VASP default of 1. Changing the dielectric constant of the medium will cause results to be incompatible with MP. |
+| GGA / METAGGA | The level of theory used must match the relevant MP input set. Moreover, GGA and METAGGA should never be set simultaneously, as this has been shown to result in seriously erroneous results. See https://github.com/materialsproject/atomate2/issues/453#issuecomment-1699605867 for more details. |
+| GGA_COMPAT | GGA_COMPAT must be set to the VASP default of True. The VASP manual only recommends setting this to False for noncollinear magnetic calculations, which are not currently included in the MP database. |
+| IBRION | IBRION values must be one of: -1, 1, 2. Other IBRION values correspond to non-standard forms of DFT calculations that are not included in the MP database. (Note that, while phonon data is included in the MP database, such values are not calculated using, say, IBRION = 5. Such logic applies to all other IBRION values not allowed). |
+| ICHARG | ICHARG must be set to be compatible with the calculation type. For example, if the relevant MP input set is for a SCF calculation, ICHARG $\leq 9$ must be used. For NSCF calculations, the value for ICHARG must exactly match the value contained in the relevant MP input set. |
+| ICORELEVEL | ICORELEVEL must be set to 0. MP does not explicitly calculate core energies. |
+| IDIPOL | IDIPOL must be set to 0 (the VASP default). |
+| IMAGES | IMAGES must be set to 0 to match MP calculations. |
+| INIWAV | INIWAV must be set as the VASP default of 1 to be consistent with MP calculations. |
+| ISPIN | All values of ISPIN are allowed, though it should be noted that virtually all MP calculations permit spin symmetry breaking, and have ferromagnetic, antiferrogmanetic, or nonmagnetic ordering. |
+| ISMEAR | The appropriate ISMEAR depends on the bandgap of the material (which cannot be known a priori). As per the VASP manual: for metals (bandgap = 0), any ISMEAR value in [0, 1, 2] is acceptable. For nonmetals (bandgap > 0), any ISMEAR value in [-5, 0] is acceptable. Hence, for those who are performing normal relaxations/static calculations and want to ensure their calculations are MP-compatible, we recommend setting ISMEAR to 0. |
+| ISIF | MP allows any ISIF $\geq 2$. This value is restricted as such simply because all ISIF values $\geq 2$ output the complete stress tensor. |
+| ISYM | ISYM must be one of -1, 0, 1, 2, except for when the relevant MP input set uses a hybrid functional, in which case ISYM=3 is also allowed. |
+| ISTART | ISTART must be one of: 0, 1, 2. |
+| IVDW | IVDW must be set to 0. MP currently does not apply any vdW dispersion corrections. |
+| IWAVPR | IWAVPR must be set to 0 (the default). VASP discourages users from setting this tag. |
+| KGAMMA | KGAMMA must be set to True (the VASP default). This is only relevant when no KPOINTS file is used. |
+| KSPACING / KPOINTS | The KSPACING parameter or KPOINTS file must correspond with at least 0.9 times **the number of KPOINTS in the non-symmetry-reduced Brillouin zone specified by the relevant MP input set** (i.e., not the number of points in the irreducible wedge of the first Brillouin zone). Hence, either method of specifying the KPOINTS can be chosen. This ensures that a calculation uses a comparable number of kpoints to MP. |
+| Kpoint mesh type (for KPOINTS) | The type of Kpoint mesh must be valid for the symmetry of the crystal structure in the calculation. For example, for a hexagonal closed packed structure, one must use a $\Gamma$-centered mesh. All Kpoints generated using Pymatgen *should* be valid. |
+| LASPH | LASPH must be set to True (this is **<u>*not*</u>** the VASP default). |
+| LCALCEPS | LCALCEPS must be set to False (the VASP default). |
+| LBERRY | LBERRY must be set to False (the VASP default). |
+| LCALCPOL | LCALCPOL  must be set to False (the VASP default). |
+| LCHIMAG | LCHIMAG must be set to False (the VASP default). |
+| LCORR | LCORR must be set to True (the VASP default) for calculations with IALGO = 58. |
+| LDAU / LDAUU / LDAUJ / LDAUL / LDAUTYPE | For DFT$`+U`$ calculations, all parameters corresponding to $+U$ or $+J$ corrections must exactly match those specified in the relevant MP input set. Alternatively, LDAU = False (DFT) is always acceptable. |
+| LDIPOL | LDIPOL must be set to False (the VASP default). |
+| LMONO | LMONO must be set to False (the VASP default). |
+| LEFG | LEFG must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
+| LEPSILON | LEPSILON must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
+| LHFCALC | The value of LHFCALC should match that of the relevant MP input set, as it will otherwise result in a change in the level of theory applied in the calculation. |
+| LHYPERFINE | LHYPERFINE must be set to False (the VASP default). |
+| LKPROJ | LKPROJ must be set to False (the VASP default). |
+| LKPOINTS_OPT | LKPOINTS_OPT must be set to False. |
+| LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that “Energies should be evaluated with the default setting for LMAXPAW”. |
+| LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the “bench_vasp_pars.docx” document in https://github.com/materialsproject/pymatgen/issues/3322. |
+| LMAXTAU | LMAXTAU must be set to 6 (the VASP default when using LASPH = True). |
+| LMP2LT / LSMP2LT | Both must be set to False (VASP defaults) |
+| LNONCOLLINEAR / LSORBIT | Both must be set to False (VASP defaults) |
+| LOCPROJ | LOCPROJ must be set to None (the VASP default). |
+| LOPTICS | LOPTICS must be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
+| LORBIT | LORBIT must **<u>*not*</u>** be None if the user also sets ISPIN=2, otherwise all values of LORBIT are acceptable. This is due to magnetization values not being output when ISPIN=2 and LORBIT = None are set together. |
+| LREAL | If the LREAL in the relevant MP input set is “Auto”, then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
+| LRPA | LRPA must be set to False (the VASP default). MP does not currently support random phase approximation (RPA) calculations. |
+| LSPECTRAL | LSPECTRAL must be set to False (the VASP default for most calculations). |
+| LSUBROT | LSUBROT must be set to False (the VASP default). |
+| MAGMOM | While any initial magnetic moments are allowed, the final total magnetic moment for any given atom must be less than 5 $\mu_B$ (Bohr magnetons) (except for elements Gd and Eu, which must be less than 10 $\mu_B$). This simply serves as a filter for erroneous data. |
+| ML_LMFF | ML_LMFF must be set to False (the VASP default). |
+| NGX / NGY / NGZ | The values for NGX/NGY/NGZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
+| NGFX / NGFY / NGFZ | The values for NGFX/NGFY/NGFZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
+| NLSPLINE | NLSPLINE should be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
+| NBANDS | NBANDS must be greater than the value $\mathrm{ceil}(\mathrm{NELECT}/2) + 1 $(minimum allowable number of bands to avoid degeneracy) and less than 4 times (minimum allowable number of bands to avoid degeneracy). For high-throughput calculations, it is generally recommended to not set this parameter directly. See https://github.com/materialsproject/custodian/issues/224 for more information. |
+| NELECT | NELECT must not be changed from the default value VASP would use for the particular structure and pseudopotentials calculated. The easiest way to ensure that NELECT is compliant with MP data is to simply not specify NELECT in the INCAR file. |
+| NWRITE | NWRITE must be set to be $\geq 2$ (the VASP default is 2). |
+| POTIM | POTIM $\leq 5$. We suggest not setting POTIM in the INCAR file, and rather allowing VASP to set it to the default value of 0.5. |
+| PSTRESS | PSTRESS must be set to exactly 0.0 (the VASP default). |
+| PREC | PREC must be one of: "High", "Accurate". |
+| ROPT | ROPT should be set to be less than or equal to the default ROPT value (which is set based on the PREC tag). Hence, it is recommended to not set the ROPT tag in the INCAR file. |
+| RWIGS | RWIGS should not be set in the INCAR file. |
+| SCALEE | SCALEE should not be set in the INCAR file. |
+| SYMPREC | SYMPREC must be less than or equal to 1e-3 (as this is the maximum value that the Custodian package will set SYMPREC as of March 2024). For general use, we recommend leaving SYMPREC as the default generated by your desired MP input set. |
+| SIGMA | There are several rules for setting SIGMA:  <ol> <li> SIGMA  must be $\leq 0.05$ for non-metals (bandgap $>  0$). </li> <li> SIGMA must be $\leq 0.2$ for a metal (bandgap = 0). </li> <li> For metals, the SIGMA value must be small enough that the entropy term in the energy is $\leq$ 1 meV/atom (as suggested by the VASP manual). </li> </ol> |
+| VCA | MP data does not include Virtual Crystal Approximation (VCA) calculations from VASP. As such, this parameter should not be set. |
+| VASP version | The following versions of VASP are allowed: 5.4.4 or $>$ 6.0.0. For example, versions $<=$ 5.4.3 are not allowed, whereas version 6.3.1 is allowed. |
```

### Comparing `pymatgen-io-validation-0.0.1/pyproject.toml` & `pymatgen_io_validation-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   "numpy",
   "requests",
 ]
 description = "A comprehensive I/O validator for electronic structure calculations"
 dynamic = ["version"]
 keywords = ["io", "validation", "dft", "vasp"]
 license = { text = "modified BSD" }
-name = "test-validation"
+name = "pymatgen-io-validation"
 readme = "README.md"
 requires-python = '>=3.8'
 
 [project.optional-dependencies]
 dev = ["pre-commit>=2.12.1"]
 #docs = ["jupyter-book>=0.13.1",]
```

### Comparing `pymatgen-io-validation-0.0.1/setup.cfg` & `pymatgen_io_validation-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pymatgen-io-validation-0.0.1/setup.py` & `pymatgen_io_validation-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 with open(os.path.join(SETUP_PTH, "README.md")) as f:
     desc = f.read()
 
 
 setup(
     name="pymatgen-io-validation",
     packages=find_namespace_packages(include=["pymatgen.io.*"]),
-    version="0.0.1",
+    version="0.0.2",
     install_requires=["pymatgen>=2022.0.3", "emmet-core>=0.77.1", "pydantic>=2.4.2", "requests>=2.28.1"],
     extras_require={},
     package_data={"pymatgen.io.validation": ["*.yaml"]},
     author="Matthew Kuner, Janosh Riebesell, Jason Munro, Aaron Kaplan",
     author_email="matthewkuner@berkeley.edu",
     maintainer="Matthew Kuner",
-    url="https://github.com/matthewkuner/pymatgen-io-validation",
+    url="https://github.com/materialsproject/pymatgen-io-validation",
     license="BSD",
     description="A comprehensive I/O validator for electronic structure calculations",
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     keywords=["pymatgen"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
```

### Comparing `pymatgen-io-validation-0.0.1/tests/test_validation.py` & `pymatgen_io_validation-0.0.2/tests/test_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import copy
-from conftest import get_test_object
+from conftest import get_test_object, test_data_task_docs
 from pymatgen.io.validation import ValidationDoc
 from emmet.core.tasks import TaskDoc
 from monty.serialization import loadfn
 from pymatgen.core.structure import Structure
 from pymatgen.io.vasp import Kpoints
 
 ### TODO: add tests for many other MP input sets (e.g. MPNSCFSet, MPNMRSet, MPScanRelaxSet, Hybrid sets, etc.)
@@ -15,23 +15,24 @@
 
 
 def run_check(
     task_doc,
     error_message_to_search_for: str,
     should_the_check_pass: bool,
     vasprun_parameters_to_change: dict = {},  # for changing the parameters read from vasprun.xml
-    incar_settings_to_change: dict = {},  # for directly changing the INCAR file
+    incar_settings_to_change: dict = {},  # for directly changing the INCAR file,
+    validation_doc_kwargs: dict = {},  # any kwargs to pass to the ValidationDoc class
 ):
     for key, value in vasprun_parameters_to_change.items():
         task_doc.input.parameters[key] = value
 
     for key, value in incar_settings_to_change.items():
         task_doc.calcs_reversed[0].input.incar[key] = value
 
-    validation_doc = ValidationDoc.from_task_doc(task_doc)
+    validation_doc = ValidationDoc.from_task_doc(task_doc, **validation_doc_kwargs)
     has_specified_error = any([error_message_to_search_for in reason for reason in validation_doc.reasons])
 
     assert (not has_specified_error) if should_the_check_pass else has_specified_error
 
 
 @pytest.mark.parametrize(
     "object_name",
@@ -40,15 +41,15 @@
     ],
 )
 def test_validation_doc_from_directory(test_dir, object_name):
     test_object = get_test_object(object_name)
     dir_name = test_dir / "vasp" / test_object.folder
     test_validation_doc = ValidationDoc.from_directory(dir_name=dir_name)
 
-    task_doc = TaskDoc.from_directory(dir_name)
+    task_doc = test_data_task_docs[object_name]
     valid_validation_doc = ValidationDoc.from_task_doc(task_doc)
 
     # The attributes below will always be different because the objects are created at
     # different times. Hence, ignore before checking.
     delattr(test_validation_doc.builder_meta, "build_date")
     delattr(test_validation_doc, "last_updated")
     delattr(valid_validation_doc.builder_meta, "build_date")
@@ -60,17 +61,16 @@
 @pytest.mark.parametrize(
     "object_name",
     [
         pytest.param("SiOptimizeDouble", id="SiOptimizeDouble"),
     ],
 )
 def test_potcar_validation(test_dir, object_name):
-    test_object = get_test_object(object_name)
-    dir_name = test_dir / "vasp" / test_object.folder
-    task_doc = TaskDoc.from_directory(dir_name)
+
+    task_doc = test_data_task_docs[object_name]
 
     correct_potcar_summary_stats = loadfn(test_dir / "vasp" / "Si_potcar_spec.json.gz")
 
     # Check POTCAR (this test should PASS, as we ARE using a MP-compatible pseudopotential)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.calcs_reversed[0].input.potcar_spec = correct_potcar_summary_stats
     run_check(temp_task_doc, "PSEUDOPOTENTIALS", True)
@@ -87,17 +87,15 @@
     "object_name",
     [
         pytest.param("SiOptimizeDouble", id="SiOptimizeDouble"),
         pytest.param("SiStatic", id="SiStatic"),
     ],
 )
 def test_scf_incar_checks(test_dir, object_name):
-    test_object = get_test_object(object_name)
-    dir_name = test_dir / "vasp" / test_object.folder
-    task_doc = TaskDoc.from_directory(dir_name)
+    task_doc = test_data_task_docs[object_name]
     task_doc.calcs_reversed[0].output.structure._charge = 0.0  # patch for old test files
 
     # Pay *very* close attention to whether a tag is modified in the incar or in the vasprun.xml's parameters!
     # Some parameters are validated from one or the other of these items, depending on whether VASP
     # changes the value between the INCAR and the vasprun.xml (which it often does)
 
     list_of_checks = loadfn(test_dir / "vasp" / "scf_incar_check_list.yaml")
@@ -307,18 +305,16 @@
 
 @pytest.mark.parametrize(
     "object_name",
     [
         pytest.param("SiNonSCFUniform", id="SiNonSCFUniform"),
     ],
 )
-def test_nscf_incar_checks(test_dir, object_name):
-    test_object = get_test_object(object_name)
-    dir_name = test_dir / "vasp" / test_object.folder
-    task_doc = TaskDoc.from_directory(dir_name)
+def test_nscf_incar_checks(object_name):
+    task_doc = test_data_task_docs[object_name]
     task_doc.calcs_reversed[0].output.structure._charge = 0.0  # patch for old test files
 
     # ICHARG check
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.input.parameters["ICHARG"] = 11
     run_check(temp_task_doc, "ICHARG", True)
 
@@ -334,18 +330,16 @@
 
 @pytest.mark.parametrize(
     "object_name",
     [
         pytest.param("SiNonSCFUniform", id="SiNonSCFUniform"),
     ],
 )
-def test_nscf_kpoints_checks(test_dir, object_name):
-    test_object = get_test_object(object_name)
-    dir_name = test_dir / "vasp" / test_object.folder
-    task_doc = TaskDoc.from_directory(dir_name)
+def test_nscf_kpoints_checks(object_name):
+    task_doc = test_data_task_docs[object_name]
     task_doc.calcs_reversed[0].output.structure._charge = 0.0  # patch for old test files
 
     # Explicit kpoints for NSCF calc check (this should not raise any flags for NSCF calcs)
     temp_task_doc = copy.deepcopy(task_doc)
     _update_kpoints_for_test(
         temp_task_doc,
         {
@@ -363,18 +357,16 @@
 @pytest.mark.parametrize(
     "object_name",
     [
         pytest.param("SiOptimizeDouble", id="SiOptimizeDouble"),
         # pytest.param("SiStatic", id="SiStatic"),
     ],
 )
-def test_common_error_checks(test_dir, object_name):
-    test_object = get_test_object(object_name)
-    dir_name = test_dir / "vasp" / test_object.folder
-    task_doc = TaskDoc.from_directory(dir_name)
+def test_common_error_checks(object_name):
+    task_doc = test_data_task_docs[object_name]
     task_doc.calcs_reversed[0].output.structure._charge = 0.0  # patch for old test files
 
     # METAGGA and GGA tag check (should never be set together)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.calcs_reversed[0].input.incar["METAGGA"] = "R2SCAN"
     temp_task_doc.calcs_reversed[0].input.incar["GGA"] = "PE"
     run_check(temp_task_doc, "KNOWN BUG", False)
@@ -457,18 +449,16 @@
 
 @pytest.mark.parametrize(
     "object_name",
     [
         pytest.param("SiOptimizeDouble", id="SiOptimizeDouble"),
     ],
 )
-def test_kpoints_checks(test_dir, object_name):
-    test_object = get_test_object(object_name)
-    dir_name = test_dir / "vasp" / test_object.folder
-    task_doc = TaskDoc.from_directory(dir_name)
+def test_kpoints_checks(object_name):
+    task_doc = test_data_task_docs[object_name]
     task_doc.calcs_reversed[0].output.structure._charge = 0.0  # patch for old test files
 
     # Valid mesh type check (should flag HCP structures)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.calcs_reversed[0].input.structure = Structure(
         lattice=[[0.5, -0.866025403784439, 0], [0.5, 0.866025403784439, 0], [0, 0, 1.6329931618554521]],
         coords=[[0, 0, 0], [0.333333333333333, -0.333333333333333, 0.5]],
@@ -520,18 +510,16 @@
 
 @pytest.mark.parametrize(
     "object_name",
     [
         pytest.param("SiOptimizeDouble", id="SiOptimizeDouble"),
     ],
 )
-def test_vasp_version_check(test_dir, object_name):
-    test_object = get_test_object(object_name)
-    dir_name = test_dir / "vasp" / test_object.folder
-    task_doc = TaskDoc.from_directory(dir_name)
+def test_vasp_version_check(object_name):
+    task_doc = test_data_task_docs[object_name]
     task_doc.calcs_reversed[0].output.structure._charge = 0.0  # patch for old test files
 
     vasp_version_list = [
         {"vasp_version": "4.0.0", "should_pass": False},
         {"vasp_version": "5.0.0", "should_pass": False},
         {"vasp_version": "5.4.0", "should_pass": False},
         {"vasp_version": "5.4.4", "should_pass": True},
@@ -564,14 +552,73 @@
     calcs["non-compliant"] = loadfn(
         str(test_dir / "vasp" / "TaskDocuments" / "MP_incompatible_GaAs_r2SCAN_static_TaskDocument.json.gz"), cls=None
     )
 
     valid_docs = {}
     for calc in calcs:
         valid_docs[calc] = ValidationDoc.from_task_doc(TaskDocument(**calcs[calc]))
+        # quickly check that `from_dict` and `from_task_doc` give same document
+        assert set(ValidationDoc.from_dict(calcs[calc]).reasons) == set(valid_docs[calc].reasons)
 
     assert valid_docs["compliant"].valid
     assert not valid_docs["non-compliant"].valid
 
     expected_reasons = ["KPOINTS", "ENCUT", "ENAUG"]
     for expected_reason in expected_reasons:
         assert any(expected_reason in reason for reason in valid_docs["non-compliant"].reasons)
+
+
+def test_fast_mode():
+    task_doc = test_data_task_docs["SiStatic"]
+    valid_doc = ValidationDoc.from_task_doc(task_doc, check_potcar=False)
+
+    # Without POTCAR check, this doc is valid
+    assert valid_doc.valid
+
+    # Now introduce sequence of changes to test how fast validation works
+    # Check order:
+    # 1. VASP version
+    # 2. Common errors (known bugs, missing output, etc.)
+    # 3. K-point density
+    # 4. POTCAR check
+    # 5. INCAR check
+
+    og_kpoints = task_doc.calcs_reversed[0].input.kpoints
+    # Introduce series of errors, then ablate them
+    # use unacceptable version and set METAGGA and GGA simultaneously ->
+    # should only get version error in reasons
+    task_doc.calcs_reversed[0].vasp_version = "4.0.0"
+    task_doc.input.parameters["NBANDS"] = -5
+    bad_incar_updates = {
+        "METAGGA": "R2SCAN",
+        "GGA": "PE",
+    }
+    task_doc.calcs_reversed[0].input.incar.update(bad_incar_updates)
+
+    _update_kpoints_for_test(task_doc, {"kpoints": [[1, 1, 2]]})
+
+    valid_doc = ValidationDoc.from_task_doc(task_doc, check_potcar=True, fast=True)
+    assert len(valid_doc.reasons) == 1
+    assert "VASP VERSION" in valid_doc.reasons[0]
+
+    # Now correct version, should just get METAGGA / GGA bug
+    task_doc.calcs_reversed[0].vasp_version = "6.3.2"
+    valid_doc = ValidationDoc.from_task_doc(task_doc, check_potcar=True, fast=True)
+    assert len(valid_doc.reasons) == 1
+    assert "KNOWN BUG" in valid_doc.reasons[0]
+
+    # Now remove GGA tag, get k-point density error
+    task_doc.calcs_reversed[0].input.incar.pop("GGA")
+    valid_doc = ValidationDoc.from_task_doc(task_doc, check_potcar=True, fast=True)
+    assert len(valid_doc.reasons) == 1
+    assert "INPUT SETTINGS --> KPOINTS or KSPACING:" in valid_doc.reasons[0]
+
+    # Now restore k-points and check POTCAR --> get error
+    _update_kpoints_for_test(task_doc, og_kpoints)
+    valid_doc = ValidationDoc.from_task_doc(task_doc, check_potcar=True, fast=True)
+    assert len(valid_doc.reasons) == 1
+    assert "PSEUDOPOTENTIALS" in valid_doc.reasons[0]
+
+    # Without POTCAR check, should get INCAR check error for NGX
+    valid_doc = ValidationDoc.from_task_doc(task_doc, check_potcar=False, fast=True)
+    assert len(valid_doc.reasons) == 1
+    assert "NBANDS" in valid_doc.reasons[0]
```

