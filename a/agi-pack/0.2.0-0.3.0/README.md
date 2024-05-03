# Comparing `tmp/agi_pack-0.2.0-py3-none-any.whl.zip` & `tmp/agi_pack-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17273 bytes, number of entries: 13
--rw-rw-r--  2.0 unx     8906 b- defN 23-Oct-25 18:03 agipack/builder.py
--rw-rw-r--  2.0 unx     7711 b- defN 23-Oct-23 18:10 agipack/cli.py
--rw-rw-r--  2.0 unx    10415 b- defN 24-Jan-23 02:06 agipack/config.py
--rw-rw-r--  2.0 unx      337 b- defN 23-Oct-17 18:36 agipack/constants.py
--rw-rw-r--  2.0 unx       22 b- defN 24-Jan-23 02:06 agipack/version.py
--rw-rw-r--  2.0 unx     5249 b- defN 24-Jan-19 00:01 agipack/templates/Dockerfile.j2
--rw-rw-r--  2.0 unx      226 b- defN 23-Oct-22 17:38 agipack/templates/agibuild.sample.yaml
--rw-rw-r--  2.0 unx     1070 b- defN 24-Jan-23 02:29 agi_pack-0.2.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx    11378 b- defN 24-Jan-23 02:29 agi_pack-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Jan-23 02:29 agi_pack-0.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       45 b- defN 24-Jan-23 02:29 agi_pack-0.2.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 24-Jan-23 02:29 agi_pack-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1039 b- defN 24-Jan-23 02:29 agi_pack-0.2.0.dist-info/RECORD
-13 files, 46498 bytes uncompressed, 15541 bytes compressed:  66.6%
+Zip file size: 17270 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx     8906 b- defN 24-May-03 14:59 agipack/builder.py
+-rw-rw-r--  2.0 unx     7711 b- defN 24-May-03 14:59 agipack/cli.py
+-rw-rw-r--  2.0 unx    10415 b- defN 24-May-03 14:59 agipack/config.py
+-rw-rw-r--  2.0 unx      337 b- defN 24-May-03 14:59 agipack/constants.py
+-rw-rw-r--  2.0 unx       22 b- defN 24-May-03 19:57 agipack/version.py
+-rw-rw-r--  2.0 unx     5277 b- defN 24-May-03 20:06 agipack/templates/Dockerfile.j2
+-rw-rw-r--  2.0 unx      226 b- defN 24-May-03 14:59 agipack/templates/agibuild.sample.yaml
+-rw-rw-r--  2.0 unx     1070 b- defN 24-May-03 20:12 agi_pack-0.3.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    11378 b- defN 24-May-03 20:12 agi_pack-0.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-03 20:12 agi_pack-0.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       45 b- defN 24-May-03 20:12 agi_pack-0.3.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 24-May-03 20:12 agi_pack-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1039 b- defN 24-May-03 20:12 agi_pack-0.3.0.dist-info/RECORD
+13 files, 46526 bytes uncompressed, 15538 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: agipack/templates/Dockerfile.j2
 Comment: 
 
 Filename: agipack/templates/agibuild.sample.yaml
 Comment: 
 
-Filename: agi_pack-0.2.0.dist-info/LICENSE
+Filename: agi_pack-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: agi_pack-0.2.0.dist-info/METADATA
+Filename: agi_pack-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: agi_pack-0.2.0.dist-info/WHEEL
+Filename: agi_pack-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: agi_pack-0.2.0.dist-info/entry_points.txt
+Filename: agi_pack-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: agi_pack-0.2.0.dist-info/top_level.txt
+Filename: agi_pack-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: agi_pack-0.2.0.dist-info/RECORD
+Filename: agi_pack-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agipack/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.0"
+__version__ = "0.3.0"
```

## agipack/templates/Dockerfile.j2

```diff
@@ -55,23 +55,24 @@
     && echo "system install complete"
 
 {%- endif %}
 
 
 {%- if is_base_image %}
 
-# Install mambaforge, with cache mounting ${CONDA_PKGS_DIRS} for faster builds
+# Install miniconda, with cache mounting ${CONDA_PKGS_DIRS} for faster builds
 RUN --mount=type=cache,target=${CONDA_PKGS_DIRS} \
-  curl -sLo ~/mambaforge.sh "https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-$(uname)-$(uname -m).sh" \
-  && chmod +x ~/mambaforge.sh \
-  && ~/mambaforge.sh -b -p ${AGIPACK_PATH}/conda \
-  && ${AGIPACK_PATH}/conda/bin/mamba init bash \
-  && ${AGIPACK_PATH}/conda/bin/mamba config --add channels conda-forge \
-  && ${AGIPACK_PATH}/conda/bin/mamba create -n ${AGIPACK_PYENV} python=${PYTHON_VERSION} -y \
-  && rm ~/mambaforge.sh
+  curl -sLo ~/miniconda.sh "https://repo.anaconda.com/miniconda/Miniconda3-latest-$(uname)-$(uname -m).sh" \
+  && chmod +x ~/miniconda.sh \
+  && ~/miniconda.sh -b -p ${AGIPACK_PATH}/conda \
+  && ${AGIPACK_PATH}/conda/bin/conda init bash \
+  && ${AGIPACK_PATH}/conda/bin/conda config --add channels conda-forge \
+  && ${AGIPACK_PATH}/conda/bin/conda create -n ${AGIPACK_PYENV} python=${PYTHON_VERSION} -y \
+  && ${AGIPACK_PATH}/conda/bin/conda install mamba -y \
+  && rm ~/miniconda.sh
 
 # Upgrade pip
 RUN pip install --upgrade pip
 {%- endif %}
 
 
 {%- if conda|length > 0 %}
```

## Comparing `agi_pack-0.2.0.dist-info/LICENSE` & `agi_pack-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `agi_pack-0.2.0.dist-info/METADATA` & `agi_pack-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agi-pack
-Version: 0.2.0
+Version: 0.3.0
 Summary: Dockerfile generator for AGI -- nothing more, nothing less.
 License: MIT License
         
         Copyright (c) 2023 Sudeep Pillai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agi-pack Version: 0.2.0 Summary: Dockerfile
+Metadata-Version: 2.1 Name: agi-pack Version: 0.3.0 Summary: Dockerfile
 generator for AGI -- nothing more, nothing less. License: MIT License Copyright
 (c) 2023 Sudeep Pillai Permission is hereby granted, free of charge, to any
 person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

## Comparing `agi_pack-0.2.0.dist-info/RECORD` & `agi_pack-0.3.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 agipack/builder.py,sha256=4qn1RrPkW-EU9osyihjYpXsH-V2LMyfeM76guHRYrGU,8906
 agipack/cli.py,sha256=KomnLpzJwwQ7fjofk1esN1Rhaodnd0LdzoAXGd8k0cY,7711
 agipack/config.py,sha256=Pg1T4qHqPdhWdAhKYaqIWKQfGw8yX52ahPLBmkCmXKw,10415
 agipack/constants.py,sha256=cnUn5DQF9la7z05dJrYPVdf0qmX3MV2Mkfog_SFLIoY,337
-agipack/version.py,sha256=Zn1KFblwuFHiDRdRAiRnDBRkbPttWh44jKa5zG2ov0E,22
-agipack/templates/Dockerfile.j2,sha256=O0ydt7s3fRsJGI-X1PKsPKINaTIWtX5A45zFca_V3AM,5249
+agipack/version.py,sha256=VrXpHDu3erkzwl_WXrqINBm9xWkcyUy53IQOj042dOs,22
+agipack/templates/Dockerfile.j2,sha256=fRBiC-AxdLMI8bbTxBJj4Ip6PaM5pFPzD1C41swIypc,5277
 agipack/templates/agibuild.sample.yaml,sha256=ysP_bpGeMGKPr3LqfzLhvEKPNJ86jVVeW66XjRxvut8,226
-agi_pack-0.2.0.dist-info/LICENSE,sha256=XtjSX1x06EhVZr1WvH_-AdrcfzmQ_Px2yawjdgmwA_E,1070
-agi_pack-0.2.0.dist-info/METADATA,sha256=0Bbf0F8pgKJerG_k5IHM2DOG8xLv8fybL-QX-0LCI0U,11378
-agi_pack-0.2.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-agi_pack-0.2.0.dist-info/entry_points.txt,sha256=7mLhXFt8cKyG7XwcK7zwQKWpDvC3Wuj_f3WQG2S5uaU,45
-agi_pack-0.2.0.dist-info/top_level.txt,sha256=MdExAigXNzVF6N8W57fUAeHe5h3ygBijmKNRuJa2fnM,8
-agi_pack-0.2.0.dist-info/RECORD,,
+agi_pack-0.3.0.dist-info/LICENSE,sha256=XtjSX1x06EhVZr1WvH_-AdrcfzmQ_Px2yawjdgmwA_E,1070
+agi_pack-0.3.0.dist-info/METADATA,sha256=z-WbWq8RUsg7Ll65pr_gHj-9QkRfMy9MNiQuGrUjzQs,11378
+agi_pack-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+agi_pack-0.3.0.dist-info/entry_points.txt,sha256=7mLhXFt8cKyG7XwcK7zwQKWpDvC3Wuj_f3WQG2S5uaU,45
+agi_pack-0.3.0.dist-info/top_level.txt,sha256=MdExAigXNzVF6N8W57fUAeHe5h3ygBijmKNRuJa2fnM,8
+agi_pack-0.3.0.dist-info/RECORD,,
```

