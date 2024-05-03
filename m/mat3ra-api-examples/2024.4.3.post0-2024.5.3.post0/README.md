# Comparing `tmp/mat3ra-api-examples-2024.4.3.post0.tar.gz` & `tmp/mat3ra_api_examples-2024.5.3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra-api-examples-2024.4.3.post0.tar", last modified: Wed Apr  3 18:31:48 2024, max compression
+gzip compressed data, was "mat3ra_api_examples-2024.5.3.post0.tar", last modified: Fri May  3 02:28:16 2024, max compression
```

## Comparing `mat3ra-api-examples-2024.4.3.post0.tar` & `mat3ra_api_examples-2024.5.3.post0.tar`

### file list

```diff
@@ -1,138 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.118079 mat3ra-api-examples-2024.4.3.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.github/workflows/check_links.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.github/workflows/zip_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.lycheeignore
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/Si.pz-vbc.UPF
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/bash_workflow_template.json
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/mp-978534.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/examples/job/
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.py
--rw-r--r--   0 runner    (1001) docker     (127)    21116 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/examples/material/
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/examples/system/
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/examples/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.122079 mat3ra-api-examples-2024.4.3.post0/extra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/extra/css/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/extra/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/images/
--rw-r--r--   0 runner    (1001) docker     (127)   413869 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/images/reusable-kernel.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/other/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   638208 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/bitter-sweet.csv
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/bittersweet_xgboost.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/deepchem_smiles_vocab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/gamma_alumina_digne_et_al.poscar
--rwxr-xr-x   0 runner    (1001) docker     (127)    12157 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/sci_adv_dean_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24590 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24267 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24750 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Gr.json
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Ni.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/jarvis/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/job/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/job/Smiles_Generation_Markov_Chain.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/job/Smiles_Generation_Markov_Chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/neural_network_train.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/neural_network_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16800 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30016 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_materials_from_files.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/uploads/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/uploads/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/1_layer_on_substrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/2_strain_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/3_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/4_custom_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/other/webinar/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/adsorption-study.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/adsorption-study.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/generate-al2o3-slab-structures.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/generate-al2o3-slab-structures.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/predict_with_machine_learning.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/predict_with_machine_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/scripts/change-branch-in-urls.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/scripts/env.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2267 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/scripts/render-notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/jupyterlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/utils/web/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/web/renderjson.css
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/web/renderjson.js
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/wheel_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.876279 mat3ra_api_examples-2024.5.3.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.856279 mat3ra_api_examples-2024.5.3.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.860279 mat3ra_api_examples-2024.5.3.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/.github/workflows/check_links.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/.github/workflows/zip_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/.lycheeignore
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-03 02:28:16.876279 mat3ra_api_examples-2024.5.3.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/README.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.860279 mat3ra_api_examples-2024.5.3.post0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.860279 mat3ra_api_examples-2024.5.3.post0/examples/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/assets/Si.pz-vbc.UPF
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/assets/bash_workflow_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/assets/mp-978534.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.860279 mat3ra_api_examples-2024.5.3.post0/examples/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/job/create_and_submit_job.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/job/create_and_submit_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/job/get-file-from-job.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/job/get-file-from-job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21116 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/job/ml-train-model-predict-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/job/ml-train-model-predict-properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/job/run-simulations-and-extract-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/job/run-simulations-and-extract-properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.864279 mat3ra_api_examples-2024.5.3.post0/examples/material/
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/material/create_material.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/material/create_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/material/get_materials_by_formula.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/material/get_materials_by_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/material/upload_materials_from_file_poscar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/material/upload_materials_from_file_poscar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.864279 mat3ra_api_examples-2024.5.3.post0/examples/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/system/get_authentication_params.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/system/get_authentication_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.864279 mat3ra_api_examples-2024.5.3.post0/examples/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/workflow/get_workflows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/workflow/get_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/workflow/qe_scf_calculation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/examples/workflow/qe_scf_calculation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.856279 mat3ra_api_examples-2024.5.3.post0/extra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.864279 mat3ra_api_examples-2024.5.3.post0/extra/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/extra/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.864279 mat3ra_api_examples-2024.5.3.post0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   413869 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/images/reusable-kernel.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.876279 mat3ra_api_examples-2024.5.3.post0/mat3ra_api_examples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-03 02:28:16.000000 mat3ra_api_examples-2024.5.3.post0/mat3ra_api_examples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-03 02:28:16.000000 mat3ra_api_examples-2024.5.3.post0/mat3ra_api_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:28:16.000000 mat3ra_api_examples-2024.5.3.post0/mat3ra_api_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 02:28:16.000000 mat3ra_api_examples-2024.5.3.post0/mat3ra_api_examples.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-03 02:28:16.000000 mat3ra_api_examples-2024.5.3.post0/mat3ra_api_examples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 02:28:16.000000 mat3ra_api_examples-2024.5.3.post0/mat3ra_api_examples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.864279 mat3ra_api_examples-2024.5.3.post0/other/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.868279 mat3ra_api_examples-2024.5.3.post0/other/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   638208 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/assets/bitter-sweet.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/assets/bittersweet_xgboost.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/assets/deepchem_smiles_vocab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/assets/gamma_alumina_digne_et_al.poscar
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12157 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/assets/sci_adv_dean_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.868279 mat3ra_api_examples-2024.5.3.post0/other/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24590 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24267 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24750 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.868279 mat3ra_api_examples-2024.5.3.post0/other/experiments/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/experiments/uploads/Gr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/experiments/uploads/Ni.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.868279 mat3ra_api_examples-2024.5.3.post0/other/jarvis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.868279 mat3ra_api_examples-2024.5.3.post0/other/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/job/Smiles_Generation_Markov_Chain.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/job/Smiles_Generation_Markov_Chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.868279 mat3ra_api_examples-2024.5.3.post0/other/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/machine_learning/neural_network_train.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/machine_learning/neural_network_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.868279 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30016 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/import_materials_from_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.872279 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.872279 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materials_designer/uploads/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.872279 mat3ra_api_examples-2024.5.3.post0/other/materialsproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materialsproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materialsproject/api_interoperability_showcase.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materialsproject/api_interoperability_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materialsproject/import_materials_from_materialsproject.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/materialsproject/import_materials_from_materialsproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.872279 mat3ra_api_examples-2024.5.3.post0/other/python_transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/python_transformations/1_layer_on_substrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/python_transformations/2_strain_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/python_transformations/3_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/python_transformations/4_custom_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/python_transformations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.872279 mat3ra_api_examples-2024.5.3.post0/other/webinar/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/webinar/adsorption-study.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/webinar/adsorption-study.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/webinar/generate-al2o3-slab-structures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/webinar/generate-al2o3-slab-structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/webinar/predict_with_machine_learning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/webinar/predict_with_machine_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.872279 mat3ra_api_examples-2024.5.3.post0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/scripts/change-branch-in-urls.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/scripts/env.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2267 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/scripts/render-notebooks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:28:16.876279 mat3ra_api_examples-2024.5.3.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.876279 mat3ra_api_examples-2024.5.3.post0/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/jupyterlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:28:16.876279 mat3ra_api_examples-2024.5.3.post0/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/web/renderjson.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/utils/web/renderjson.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-03 02:27:43.000000 mat3ra_api_examples-2024.5.3.post0/wheel_server.py
```

### Comparing `mat3ra-api-examples-2024.4.3.post0/.gitattributes` & `mat3ra_api_examples-2024.5.3.post0/.gitattributes`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/.github/workflows/cicd.yml` & `mat3ra_api_examples-2024.5.3.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/.github/workflows/zip_release.yml` & `mat3ra_api_examples-2024.5.3.post0/.github/workflows/zip_release.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/.gitignore` & `mat3ra_api_examples-2024.5.3.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/PKG-INFO` & `mat3ra_api_examples-2024.5.3.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mat3ra-api-examples
-Version: 2024.4.3.post0
+Version: 2024.5.3.post0
 Summary: Mat3ra API Examples
 Project-URL: homepage, https://exabyte-io.github.io/api-examples
 Project-URL: documentation, https://exabyte-io.github.io/api-examples
 Project-URL: repository, https://github.com/Exabyte-io/api-examples
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ase>=3.21.1
 Requires-Dist: exabyte-api-client>=2023.6.13.post0
 Requires-Dist: matplotlib>=3.4.1
 Requires-Dist: pandas>=1.5.3
-Requires-Dist: pymatgen>=2023.5.31
+Requires-Dist: pymatgen>=2024.4.13
+Requires-Dist: mat3ra-made>=2024.5.3.post0
 Provides-Extra: colab
 Requires-Dist: mat3ra-api-examples; extra == "colab"
 Provides-Extra: jupyterlab
 Requires-Dist: jupyterlab>=3.0.17; extra == "jupyterlab"
 Requires-Dist: nbconvert>=6.0.7; extra == "jupyterlab"
 Provides-Extra: localhost
 Requires-Dist: mat3ra-api-examples[jupyterlab]; extra == "localhost"
```

### Comparing `mat3ra-api-examples-2024.4.3.post0/README.md` & `mat3ra_api_examples-2024.5.3.post0/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/config.yml` & `mat3ra_api_examples-2024.5.3.post0/config.yml`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,18 @@
   - name: create_interface_with_min_strain_zsl.ipynb
     packages_common:
       - ipywidgets
       - plotly==5.18
       - nbformat>=4.2.0
     packages_python:
     packages_pyodide:
+      - annotated_types>=0.6.0
+      - https://files.mat3ra.com/uploads/pydantic_core-2.18.2-py3-none-any.whl
+      - https://files.mat3ra.com/uploads/pydantic-2.7.1-py3-none-any.whl
+      - mat3ra-made
   - name: import_material_from_jarvis_db_entry.ipynb
     packages_common:
       - express-py==2024.2.2.post2
       - mat3ra-esse
       - jarvis-tools
       - munch
       - setuptools
```

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/assets/bash_workflow_template.json` & `mat3ra_api_examples-2024.5.3.post0/examples/assets/bash_workflow_template.json`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/config.py` & `mat3ra_api_examples-2024.5.3.post0/examples/config.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/job/create_and_submit_job.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.py` & `mat3ra_api_examples-2024.5.3.post0/examples/job/create_and_submit_job.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/job/get-file-from-job.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.py` & `mat3ra_api_examples-2024.5.3.post0/examples/job/get-file-from-job.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/job/ml-train-model-predict-properties.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.py` & `mat3ra_api_examples-2024.5.3.post0/examples/job/ml-train-model-predict-properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/job/run-simulations-and-extract-properties.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.py` & `mat3ra_api_examples-2024.5.3.post0/examples/job/run-simulations-and-extract-properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/material/create_material.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.py` & `mat3ra_api_examples-2024.5.3.post0/examples/material/create_material.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/material/get_materials_by_formula.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.py` & `mat3ra_api_examples-2024.5.3.post0/examples/material/get_materials_by_formula.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/material/upload_materials_from_file_poscar.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.py` & `mat3ra_api_examples-2024.5.3.post0/examples/material/upload_materials_from_file_poscar.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/system/get_authentication_params.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.py` & `mat3ra_api_examples-2024.5.3.post0/examples/system/get_authentication_params.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/workflow/get_workflows.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.py` & `mat3ra_api_examples-2024.5.3.post0/examples/workflow/get_workflows.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.ipynb` & `mat3ra_api_examples-2024.5.3.post0/examples/workflow/qe_scf_calculation.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.py` & `mat3ra_api_examples-2024.5.3.post0/examples/workflow/qe_scf_calculation.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/images/reusable-kernel.png` & `mat3ra_api_examples-2024.5.3.post0/images/reusable-kernel.png`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/PKG-INFO` & `mat3ra_api_examples-2024.5.3.post0/mat3ra_api_examples.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mat3ra-api-examples
-Version: 2024.4.3.post0
+Version: 2024.5.3.post0
 Summary: Mat3ra API Examples
 Project-URL: homepage, https://exabyte-io.github.io/api-examples
 Project-URL: documentation, https://exabyte-io.github.io/api-examples
 Project-URL: repository, https://github.com/Exabyte-io/api-examples
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ase>=3.21.1
 Requires-Dist: exabyte-api-client>=2023.6.13.post0
 Requires-Dist: matplotlib>=3.4.1
 Requires-Dist: pandas>=1.5.3
-Requires-Dist: pymatgen>=2023.5.31
+Requires-Dist: pymatgen>=2024.4.13
+Requires-Dist: mat3ra-made>=2024.5.3.post0
 Provides-Extra: colab
 Requires-Dist: mat3ra-api-examples; extra == "colab"
 Provides-Extra: jupyterlab
 Requires-Dist: jupyterlab>=3.0.17; extra == "jupyterlab"
 Requires-Dist: nbconvert>=6.0.7; extra == "jupyterlab"
 Provides-Extra: localhost
 Requires-Dist: mat3ra-api-examples[jupyterlab]; extra == "localhost"
```

### Comparing `mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/SOURCES.txt` & `mat3ra_api_examples-2024.5.3.post0/mat3ra_api_examples.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitattributes
 .gitignore
 .lycheeignore
 .pre-commit-config.yaml
+README.ipynb
 README.md
 config.yml
 mkdocs.yml
 pyproject.toml
 wheel_server.py
 .github/workflows/check_links.yml
 .github/workflows/cicd.yml
@@ -98,11 +99,12 @@
 scripts/env.sh
 scripts/render-notebooks.sh
 utils/__init__.py
 utils/generic.py
 utils/jupyterlite.py
 utils/material.py
 utils/notebook.py
+utils/plot.py
 utils/settings.json
 utils/settings.py
 utils/web/renderjson.css
 utils/web/renderjson.js
```

### Comparing `mat3ra-api-examples-2024.4.3.post0/mkdocs.yml` & `mat3ra_api_examples-2024.5.3.post0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/assets/README.md` & `mat3ra_api_examples-2024.5.3.post0/other/assets/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/assets/bitter-sweet.csv` & `mat3ra_api_examples-2024.5.3.post0/other/assets/bitter-sweet.csv`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/assets/gamma_alumina_digne_et_al.poscar` & `mat3ra_api_examples-2024.5.3.post0/other/assets/gamma_alumina_digne_et_al.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/assets/sci_adv_dean_data.csv` & `mat3ra_api_examples-2024.5.3.post0/other/assets/sci_adv_dean_data.csv`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Gr.json` & `mat3ra_api_examples-2024.5.3.post0/other/experiments/uploads/Gr.json`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Ni.json` & `mat3ra_api_examples-2024.5.3.post0/other/experiments/uploads/Ni.json`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/job/Smiles_Generation_Markov_Chain.py` & `mat3ra_api_examples-2024.5.3.post0/other/job/Smiles_Generation_Markov_Chain.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py` & `mat3ra_api_examples-2024.5.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py` & `mat3ra_api_examples-2024.5.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/machine_learning/neural_network_train.py` & `mat3ra_api_examples-2024.5.3.post0/other/machine_learning/neural_network_train.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/Introduction.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/materials_designer/Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9812805904020414%*

 * *Differences: {"'cells'": "{2: {'source': {delete: [7, 1]}}, 7: {'source': ['## 2. Install Packages\\n', 'The "*

 * *            'step executes only in Pyodide environment. For other environments, the packages '*

 * *            "should be installed via `pip install` as directed in README.']}, 8: {'source': "*

 * *            "{insert: [(4, '    from utils.jupyterlite import install_packages\\n'), (5, '    "*

 * *            'await '*

 * *            'install_packages("create_interface_with_min_strain_zsl.ipynb","../../config.yml")\')], '*

 * *       […]*

```diff
@@ -42,21 +42,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "SUBSTRATE_PARAMETERS = {\n",
-                "    \"MATERIAL_INDEX\": 0,  # the index of the material in the materials_in list\n",
                 "    \"MILLER_INDICES\": (1, 1, 1),  # the miller indices of the interfacial plane\n",
                 "    \"THICKNESS\": 3,  # in layers\n",
                 "}\n",
                 "\n",
                 "LAYER_PARAMETERS = {\n",
-                "    \"MATERIAL_INDEX\": 1,  # the index of the material in the materials_in list\n",
                 "    \"MILLER_INDICES\": (0, 0, 1),  # the miller indices of the interfacial plane\n",
                 "    \"THICKNESS\": 1,  # in layers\n",
                 "}\n",
                 "\n",
                 "USE_CONVENTIONAL_CELL = True  # if True, the surface plane is constructed using miller indices of the conventional cell"
             ]
         },
@@ -103,60 +101,56 @@
                 "}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 2. Install Packages"
+                "## 2. Install Packages\n",
+                "The step executes only in Pyodide environment. For other environments, the packages should be installed via `pip install` as directed in README."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import sys\n",
                 "if sys.platform == \"emscripten\":\n",
                 "    import micropip\n",
                 "    await micropip.install('mat3ra-api-examples', deps=False)\n",
-                "from utils.jupyterlite import install_packages\n",
-                "await install_packages(\"create_interface_with_min_strain_zsl.ipynb\",\"../../config.yml\")"
+                "    from utils.jupyterlite import install_packages\n",
+                "    await install_packages(\"create_interface_with_min_strain_zsl.ipynb\",\"../../config.yml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 3. Load and prepare input Materials\n"
+                "## 3. Load input Materials\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from utils.jupyterlite import get_data\n",
-                "from pymatgen.analysis.structure_analyzer import SpacegroupAnalyzer\n",
-                "from src.utils import to_pymatgen\n",
+                "from mat3ra.made.material import Material\n",
                 "\n",
                 "# Get the list of input materials and load them into `materials_in` variable\n",
                 "get_data(\"materials_in\", globals())\n",
-                "\n",
-                "if \"materials_in\" in globals():\n",
-                "    pymatgen_materials = [to_pymatgen(item) for item in materials_in]\n",
-                "    if USE_CONVENTIONAL_CELL: pymatgen_materials = [SpacegroupAnalyzer(item).get_conventional_standard_structure() for\n",
-                "                                                    item in pymatgen_materials]\n",
-                "\n",
-                "    for material in pymatgen_materials:\n",
-                "        print(material, \"\\n\")"
+                "materials = []      \n",
+                "for material_config in globals()[\"materials_in\"]:\n",
+                "    print(material_config, \"\\n\")\n",
+                "    materials.append(Material(material_config))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -173,276 +167,137 @@
             "execution_count": null,
             "metadata": {
                 "tags": [],
                 "trusted": true
             },
             "outputs": [],
             "source": [
-                "from src.pymatgen_coherent_interface_builder import CoherentInterfaceBuilder, ZSLGenerator\n",
-                "from src.utils import translate_to_bottom\n",
-                "\n",
-                "# Translate the materials to the bottom of the cell to allow for multilayer heterostructures creation\n",
-                "pymatgen_materials = [translate_to_bottom(item) for item in pymatgen_materials]\n",
-                "    \n",
-                "def create_interfaces(settings):\n",
-                "    print(\"Creating interfaces...\")\n",
-                "    zsl = ZSLGenerator(\n",
-                "        max_area_ratio_tol=settings[\"ZSL_PARAMETERS\"][\"MAX_AREA_TOL\"],\n",
-                "        max_area=settings[\"ZSL_PARAMETERS\"][\"MAX_AREA\"],\n",
-                "        max_length_tol=settings[\"ZSL_PARAMETERS\"][\"MAX_LENGTH_TOL\"],\n",
-                "        max_angle_tol=settings[\"ZSL_PARAMETERS\"][\"MAX_ANGLE_TOL\"],\n",
-                "    )\n",
-                "\n",
-                "    cib = CoherentInterfaceBuilder(\n",
-                "        substrate_structure=pymatgen_materials[settings[\"SUBSTRATE_PARAMETERS\"][\"MATERIAL_INDEX\"]],\n",
-                "        film_structure=pymatgen_materials[settings[\"LAYER_PARAMETERS\"][\"MATERIAL_INDEX\"]],\n",
-                "        substrate_miller=settings[\"SUBSTRATE_PARAMETERS\"][\"MILLER_INDICES\"],\n",
-                "        film_miller=settings[\"LAYER_PARAMETERS\"][\"MILLER_INDICES\"],\n",
-                "        zslgen=zsl,\n",
-                "        strain_tol=settings[\"ZSL_PARAMETERS\"][\"STRAIN_TOL\"],\n",
-                "    )\n",
-                "\n",
-                "    # Find terminations\n",
-                "    cib._find_terminations()\n",
-                "    terminations = cib.terminations\n",
-                "\n",
-                "    # Create interfaces for each termination\n",
-                "    interfaces = {}\n",
-                "    for termination in terminations:\n",
-                "        interfaces[termination] = []\n",
-                "        for interface in cib.get_interfaces(\n",
-                "                termination,\n",
-                "                gap=settings[\"INTERFACE_PARAMETERS\"][\"DISTANCE_Z\"],\n",
-                "                film_thickness=settings[\"LAYER_PARAMETERS\"][\"THICKNESS\"],\n",
-                "                substrate_thickness=settings[\"SUBSTRATE_PARAMETERS\"][\"THICKNESS\"],\n",
-                "                in_layers=True,\n",
-                "        ):\n",
-                "            # Wrap atoms to unit cell\n",
-                "            interface[\"interface\"].make_supercell((1, 1, 1), to_unit_cell=True)\n",
-                "            interfaces[termination].append(interface)\n",
-                "    return interfaces, terminations\n",
-                "\n",
+                "from mat3ra.made.tools.build import create_interfaces\n",
                 "\n",
-                "interfaces, terminations = create_interfaces(\n",
+                "interface_data_holder = create_interfaces(\n",
+                "    substrate=materials[0],\n",
+                "    layer=materials[1],\n",
                 "    settings={\n",
                 "        \"SUBSTRATE_PARAMETERS\": SUBSTRATE_PARAMETERS,\n",
                 "        \"LAYER_PARAMETERS\": LAYER_PARAMETERS,\n",
+                "        \"USE_CONVENTIONAL_CELL\": USE_CONVENTIONAL_CELL,\n",
                 "        \"ZSL_PARAMETERS\": ZSL_PARAMETERS,\n",
                 "        \"INTERFACE_PARAMETERS\": INTERFACE_PARAMETERS,\n",
-                "    }\n",
+                "    },\n",
+                "    sort_by_strain_and_size=True,\n",
+                "    remove_duplicates=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### 5.2. Print out the interfaces and terminations"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "print(f'Found {len(terminations)} terminations')\n",
-                "for termination in terminations:\n",
-                "    print(f\"Found {len(interfaces[termination])} interfaces for\", termination, \"termination\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## 5. Sort interfaces by strain\n",
-                "\n",
-                "### 5.1. Sort all interfaces"
+                "### 4.2. Print out the interfaces and terminations"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Could be \"strain\", \"von_mises_strain\", \"mean_abs_strain\"\n",
-                "strain_mode = \"mean_abs_strain\"\n",
-                "\n",
-                "\n",
-                "# Sort interfaces by the specified strain mode and number of sites\n",
-                "def sort_interfaces(interfaces, terminations):\n",
-                "    sorted_interfaces = {}\n",
-                "    for termination in terminations:\n",
-                "        sorted_interfaces[termination] = sorted(\n",
-                "            interfaces[termination], key=lambda x: (x[strain_mode], x[\"interface\"].num_sites)\n",
-                "        )\n",
-                "    return sorted_interfaces\n",
-                "\n",
-                "\n",
-                "sorted_interfaces = sort_interfaces(interfaces, terminations)"
+                "print(\"Found terminations:\", interface_data_holder.terminations)\n",
+                "print(f\"Number of interfaces for a termination:  {len(interface_data_holder.get_interfaces_for_termination(0))}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### 5.2. Print out interfaces with lowest strain for each termination"
+                "### 4.2. Print out interfaces with the lowest strain for each termination"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "for termination in terminations:\n",
+                "for termination in interface_data_holder.terminations:\n",
                 "    print(f\"Interface with lowest strain for termination {termination} (index 0):\")\n",
-                "    first_interface = sorted_interfaces[termination][0]\n",
-                "    print(\"    strain:\", first_interface[strain_mode] * 100, \"%\")\n",
-                "    print(\"    number of atoms:\", first_interface[\"interface\"].num_sites)"
+                "    interfaces = interface_data_holder.get_interfaces_for_termination(termination)\n",
+                "    first_interface = interfaces[0]\n",
+                "    print(f\"    strain: {first_interface.get_mean_abs_strain() * 100:.3f}%\")\n",
+                "    print(\"    number of atoms:\", first_interface.num_sites)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 6. Plot the results\n",
+                "## 5. Plot the results\n",
                 "\n",
                 "Plot the number of atoms vs strain. Adjust the parameters as needed.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import plotly.graph_objs as go\n",
-                "from collections import defaultdict\n",
+                "from utils.plot import plot_strain_vs_atoms\n",
                 "\n",
                 "PLOT_SETTINGS = {\n",
                 "    \"HEIGHT\": 600,\n",
                 "    \"X_SCALE\": \"log\",  # or linear\n",
                 "    \"Y_SCALE\": \"log\",  # or linear\n",
                 "}\n",
                 "\n",
+                "plot_strain_vs_atoms(interface_data_holder, PLOT_SETTINGS)\n",
                 "\n",
-                "def plot_strain_vs_atoms(sorted_interfaces, terminations, settings):\n",
-                "    # Create a mapping from termination to its index\n",
-                "    termination_to_index = {termination: i for i, termination in enumerate(terminations)}\n",
-                "\n",
-                "    grouped_interfaces = defaultdict(list)\n",
-                "    for termination, interfaces in sorted_interfaces.items():\n",
-                "        for index, interface_data in enumerate(interfaces):\n",
-                "            strain_percentage = interface_data[\"mean_abs_strain\"] * 100\n",
-                "            num_sites = interface_data[\"interface\"].num_sites\n",
-                "            key = (strain_percentage, num_sites)\n",
-                "            grouped_interfaces[key].append((index, termination))\n",
-                "\n",
-                "    data = []\n",
-                "    for (strain, num_sites), indices_and_terminations in grouped_interfaces.items():\n",
-                "        termination_indices = defaultdict(list)\n",
-                "        for index, termination in indices_and_terminations:\n",
-                "            termination_indices[termination].append(index)\n",
-                "        all_indices = [index for indices in termination_indices.values() for index in indices]\n",
-                "        index_range = f\"{min(all_indices)}-{max(all_indices)}\" if len(all_indices) > 1 else str(min(all_indices))\n",
-                "\n",
-                "        hover_text = \"<br>-----<br>\".join(\n",
-                "            f\"Termination: {termination}<br>Termination index: {termination_to_index[termination]}<br>Interfaces Index Range: {index_range}<br>Strain: {strain:.2f}%<br>Atoms: {num_sites}\"\n",
-                "            for termination, indices in termination_indices.items()\n",
-                "        )\n",
-                "        trace = go.Scatter(\n",
-                "            x=[strain],\n",
-                "            y=[num_sites],\n",
-                "            text=[hover_text],\n",
-                "            mode=\"markers\",\n",
-                "            hoverinfo=\"text\",\n",
-                "            name=f\"Indices: {index_range}\",\n",
-                "        )\n",
-                "        data.append(trace)\n",
-                "\n",
-                "    layout = go.Layout(\n",
-                "        xaxis=dict(title=\"Strain (%)\", type=settings[\"X_SCALE\"]),\n",
-                "        yaxis=dict(title=\"Number of atoms\", type=settings[\"Y_SCALE\"]),\n",
-                "        hovermode=\"closest\",\n",
-                "        height=settings[\"HEIGHT\"],\n",
-                "        legend_title_text=\"Interfaces Index Range\",\n",
-                "    )\n",
-                "    fig = go.Figure(data=data, layout=layout)\n",
-                "    fig.show()\n",
-                "\n",
-                "\n",
-                "plot_strain_vs_atoms(sorted_interfaces, terminations, PLOT_SETTINGS)\n",
-                "\n",
-                "for i, termination in enumerate(terminations):\n",
-                "    print(f\"Termination {i}:\", termination)"
+                "print(\"Terminations: \\n\", interface_data_holder.terminations)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 7. Select the interface to pass outside this kernel\n",
-                "\n",
-                "### 7.1. Select the interface with the desired termination and strain\n",
-                "\n",
-                "The data in `sorted_interfaces` now contains an object with the following structure:\n",
+                "## 6. Select the interface to pass outside this kernel\n",
                 "\n",
-                "```json\n",
-                "{\n",
-                "    \"('C_P6/mmm_2', 'Si_R-3m_1')\": [\n",
-                "        { ...interface for ('C_P6/mmm_2', 'Si_R-3m_1') at index 0...},\n",
-                "        { ...interface for ('C_P6/mmm_2', 'Si_R-3m_1') at index 1...},\n",
-                "        ...\n",
-                "    ],\n",
-                "    \"<termination at index 1>\": [\n",
-                "        { ...interface for 'termination at index 1' at index 0...},\n",
-                "        { ...interface for 'termination at index 1' at index 1...},\n",
-                "        ...\n",
-                "    ]\n",
-                "}\n",
-                "```\n",
+                "### 6.1. Select the interface with the desired termination and strain\n",
                 "\n",
                 "Select the index for termination first, and for it - the index in the list of corresponding interfaces sorted by strain (index 0 has minimum strain)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "termination_index = 0\n",
-                "number_of_interfaces_to_include = 1\n",
-                "\n",
-                "termination = terminations[termination_index]\n",
-                "\n",
-                "selected_interfaces = sorted_interfaces[termination][:number_of_interfaces_to_include]"
+                "# Could be either the termination as tuple, e.g. `('Ni_P6/mmm_1', 'C_C2/m_2')` or its index: `0`\n",
+                "termination_or_its_index = 0\n",
+                "# select the first interface with the lowest strain and the smallest number of atoms\n",
+                "interfaces_slice_range_or_index = 0\n",
+                "selected_interfaces = interface_data_holder.get_interfaces_as_materials(termination_or_its_index, interfaces_slice_range_or_index)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### 7.2. Pass data to the outside runtime\n"
+                "### 6.2. Pass data to the outside runtime\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from src.utils import from_pymatgen\n",
                 "from utils.jupyterlite import set_data\n",
                 "\n",
-                "materials = list(map(lambda interface_config: from_pymatgen(interface_config[\"interface\"]), selected_interfaces))\n",
-                "\n",
-                "set_data(\"materials\", materials)"
+                "set_data(\"materials\", selected_interfaces)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": ".venv",
             "language": "python",
```

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_materials_from_files.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/materials_designer/import_materials_from_files.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py` & `mat3ra_api_examples-2024.5.3.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/utils.py` & `mat3ra_api_examples-2024.5.3.post0/other/materials_designer/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,16 +133,17 @@
 
     Args:
         atoms (ase.Atoms): ase.Atoms object
 
     Returns:
         Structure: pymatgen Structure object
     """
-    poscar = ase_to_poscar(atoms)
-    structure = Structure.from_str(poscar, fmt="poscar")
+
+    adaptor = AseAtomsAdaptor()
+    structure = adaptor.get_structure(atoms)
 
     return structure
 
 
 def pymatgen_to_ase(structure: Structure):
     """
     Converts a Pymatgen Structure object to an ASE Atoms object,
```

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/materialsproject/api_interoperability_showcase.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.py` & `mat3ra_api_examples-2024.5.3.post0/other/materialsproject/api_interoperability_showcase.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.ipynb` & `mat3ra_api_examples-2024.5.3.post0/other/materialsproject/import_materials_from_materialsproject.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.py` & `mat3ra_api_examples-2024.5.3.post0/other/materialsproject/import_materials_from_materialsproject.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/1_layer_on_substrate.py` & `mat3ra_api_examples-2024.5.3.post0/other/python_transformations/1_layer_on_substrate.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/2_strain_matching.py` & `mat3ra_api_examples-2024.5.3.post0/other/python_transformations/2_strain_matching.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/3_imports.py` & `mat3ra_api_examples-2024.5.3.post0/other/python_transformations/3_imports.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/4_custom_transformation.py` & `mat3ra_api_examples-2024.5.3.post0/other/python_transformations/4_custom_transformation.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/README.md` & `mat3ra_api_examples-2024.5.3.post0/other/python_transformations/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/webinar/adsorption-study.py` & `mat3ra_api_examples-2024.5.3.post0/other/webinar/adsorption-study.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/webinar/generate-al2o3-slab-structures.py` & `mat3ra_api_examples-2024.5.3.post0/other/webinar/generate-al2o3-slab-structures.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/webinar/predict_with_machine_learning.py` & `mat3ra_api_examples-2024.5.3.post0/other/webinar/predict_with_machine_learning.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.py` & `mat3ra_api_examples-2024.5.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/pyproject.toml` & `mat3ra_api_examples-2024.5.3.post0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "ase>=3.21.1",
   "exabyte-api-client>=2023.6.13.post0",
   "matplotlib>=3.4.1",
   "pandas>=1.5.3",
-  "pymatgen>=2023.5.31",
+  "pymatgen>=2024.4.13",
+  "mat3ra-made>=2024.5.3.post0",
 ]
 
 [project.optional-dependencies]
 # Install all above dependencies in colab
 colab = ["mat3ra-api-examples"]
 jupyterlab = [
   "jupyterlab>=3.0.17",
```

### Comparing `mat3ra-api-examples-2024.4.3.post0/scripts/change-branch-in-urls.sh` & `mat3ra_api_examples-2024.5.3.post0/scripts/change-branch-in-urls.sh`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/scripts/env.sh` & `mat3ra_api_examples-2024.5.3.post0/scripts/env.sh`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/scripts/render-notebooks.sh` & `mat3ra_api_examples-2024.5.3.post0/scripts/render-notebooks.sh`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/utils/generic.py` & `mat3ra_api_examples-2024.5.3.post0/utils/generic.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/utils/jupyterlite.py` & `mat3ra_api_examples-2024.5.3.post0/utils/jupyterlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,18 +142,19 @@
     Write data to the `uploads` folder in a JupyterLab environment.
     Args:
         key (string): The name under which data will be written.
         value (Any): The value to write to the `uploads` folder.
     """
     if not os.path.exists(UPLOADS_FOLDER):
         os.makedirs(UPLOADS_FOLDER)
-    file_path = os.path.join(UPLOADS_FOLDER, f"{key}.json")
-    with open(file_path, "w") as file:
-        json.dump(value, file)
-    print(f"Data for {key} written to {file_path}")
+    for item in value:
+        file_path = os.path.join(UPLOADS_FOLDER, f"{item['name']}.json")
+        with open(file_path, "w") as file:
+            json.dump(item, file)
+        print(f"Data for {key} written to {file_path}")
 
 
 def set_data(key, value):
     """
     Switch between the two functions `set_data_pyodide` and `set_data_python` based on the environment.
     Args:
         key (string): The name under which data will be written or sent.
@@ -181,15 +182,15 @@
     Read data from the `uploads` folder in a JupyterLab environment.
     Args:
         key (string): The name under which data is expected to be received.
         globals_dict (dict): A dictionary to store the received data. Defaults to None.
     """
     try:
         data_from_host = []
-        for filename in os.listdir(UPLOADS_FOLDER):
+        for filename in sorted(os.listdir(UPLOADS_FOLDER)):
             if filename.endswith(".json"):
                 with open(os.path.join(UPLOADS_FOLDER, filename), "r") as file:
                     data = json.load(file)
                 name = os.path.splitext(filename)[0]
                 print(f"Data from {name} has been read successfully.")
                 data_from_host.append(data)
         if globals_dict is not None:
```

### Comparing `mat3ra-api-examples-2024.4.3.post0/utils/material.py` & `mat3ra_api_examples-2024.5.3.post0/utils/material.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/utils/notebook.py` & `mat3ra_api_examples-2024.5.3.post0/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/utils/settings.py` & `mat3ra_api_examples-2024.5.3.post0/utils/settings.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/utils/web/renderjson.js` & `mat3ra_api_examples-2024.5.3.post0/utils/web/renderjson.js`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.3.post0/wheel_server.py` & `mat3ra_api_examples-2024.5.3.post0/wheel_server.py`

 * *Files identical despite different names*

