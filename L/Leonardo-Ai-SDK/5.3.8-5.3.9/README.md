# Comparing `tmp/Leonardo-Ai-SDK-5.3.8.tar.gz` & `tmp/Leonardo-Ai-SDK-5.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-5.3.8.tar", last modified: Mon Apr 29 05:30:57 2024, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-5.3.9.tar", last modified: Fri May  3 00:02:36 2024, max compression
```

## Comparing `Leonardo-Ai-SDK-5.3.8.tar` & `Leonardo-Ai-SDK-5.3.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.396599 Leonardo-Ai-SDK-5.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-04-29 05:30:57.396599 Leonardo-Ai-SDK-5.3.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     9937 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 05:30:57.396599 Leonardo-Ai-SDK-5.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.384599 Leonardo-Ai-SDK-5.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.384599 Leonardo-Ai-SDK-5.3.8/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-04-29 05:30:57.000000 Leonardo-Ai-SDK-5.3.8/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-29 05:30:57.000000 Leonardo-Ai-SDK-5.3.8/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 05:30:57.000000 Leonardo-Ai-SDK-5.3.8/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-29 05:30:57.000000 Leonardo-Ai-SDK-5.3.8/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 05:30:57.000000 Leonardo-Ai-SDK-5.3.8/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.388599 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.388599 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    44786 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/initimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    27064 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.388599 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.388599 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.392599 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/creategeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createlcmgeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createtexturegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createvariationnobg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createvariationunzoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createvariationupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/get3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getuserself.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getvariationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/listelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/listplatformmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/performinpaintinglcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/performinstantrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/promptimprove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/promptrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/uploadinitimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/uploadmodelasset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.396599 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/controlnet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/custom_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/lcm_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/model_asset_texture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/sd_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/sd_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/universal_upscaler_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/variation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:30:57.396599 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-04-29 05:30:44.000000 Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.279698 Leonardo-Ai-SDK-5.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-03 00:02:36.279698 Leonardo-Ai-SDK-5.3.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9937 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 00:02:36.283697 Leonardo-Ai-SDK-5.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.267697 Leonardo-Ai-SDK-5.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.271697 Leonardo-Ai-SDK-5.3.9/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-03 00:02:36.000000 Leonardo-Ai-SDK-5.3.9/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-03 00:02:36.000000 Leonardo-Ai-SDK-5.3.9/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 00:02:36.000000 Leonardo-Ai-SDK-5.3.9/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-03 00:02:36.000000 Leonardo-Ai-SDK-5.3.9/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 00:02:36.000000 Leonardo-Ai-SDK-5.3.9/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.271697 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.271697 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44786 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/initimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27064 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.271697 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.271697 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.279698 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/creategeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createlcmgeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createtexturegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createvariationnobg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createvariationunzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/get3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getuserself.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/listelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/listplatformmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/performinpaintinglcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/performinstantrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/promptimprove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/promptrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/uploadinitimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/uploadmodelasset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.279698 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/controlnet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/custom_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/lcm_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/model_asset_texture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/sd_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/universal_upscaler_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/variation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:02:36.279698 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-05-03 00:02:22.000000 Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-5.3.8/LICENSE.md` & `Leonardo-Ai-SDK-5.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/PKG-INFO` & `Leonardo-Ai-SDK-5.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.3.8
+Version: 5.3.9
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.8 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.9 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
```

### Comparing `Leonardo-Ai-SDK-5.3.8/README.md` & `Leonardo-Ai-SDK-5.3.9/README.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/setup.py` & `Leonardo-Ai-SDK-5.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='Leonardo-Ai-SDK',
-    version='5.3.8',
+    version='5.3.9',
     author='Leonardo-Ai',
     description='Leonardo AI Python Client SDK',
     url='https://github.com/Leonardo-Interactive/leonardo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `Leonardo-Ai-SDK-5.3.8/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-5.3.9/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.3.8
+Version: 5.3.9
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.8 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.9 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
```

### Comparing `Leonardo-Ai-SDK-5.3.8/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-5.3.9/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/_hooks/sdkhooks.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/_hooks/types.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/element.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/element.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/generation.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/initimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/model.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/errors/sdkerror.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     model_id: Optional[str] = dataclasses.field(default='b24e16ff-06e3-43eb-8d33-4416c2d75876', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelId'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The model ID used for image generation. If not provided, uses sd_version to determine the version of Stable Diffusion to use. In-app, model IDs are under the Finetune Models menu. Click on the platform model or your custom model, then click View More. For platform models, you can also use the List Platform Models API."""
     negative_prompt: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('negative_prompt'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The negative prompt used for the image generation"""
     num_images: Optional[int] = dataclasses.field(default=4, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_images'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The number of images to generate. Must be between 1 and 8. If either width or height is over 768, must be between 1 and 4."""
     num_inference_steps: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_inference_steps'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
-    r"""The number of inference steps to use for the generation. Must be between 30 and 60."""
+    r"""The Step Count to use for the generation. Must be between 10 and 60. Default is 15."""
     photo_real: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoReal'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable the photoReal feature. Requires enabling alchemy and unspecifying modelId (for photoRealVersion V1)."""
     photo_real_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealStrength'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Depth of field of photoReal. Must be 0.55 for low, 0.5 for medium, or 0.45 for high. Defaults to 0.55 if not specified."""
     photo_real_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealVersion'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The version of photoReal to use. Must be v1 or v2."""
     preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=shared_sd_generation_style.SdGenerationStyle.DYNAMIC, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
@@ -91,15 +91,15 @@
     unzoom: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unzoom'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Whether the generated images should be unzoomed (requires unzoomAmount and init_image_id to be set)."""
     unzoom_amount: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unzoomAmount'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How much the image should be unzoomed (requires an init_image_id and unzoom to be set to true)."""
     upscale_ratio: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('upscaleRatio'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How much the image should be upscaled. (Enterprise Only)"""
     weighting: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weighting'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
-    r"""How much weighting to use for generation."""
+    r"""How much weighting to use for ControlNet. This parameter works with controlNet and controlNetType."""
     width: Optional[int] = dataclasses.field(default=1024, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The input width of the images. Must be between 32 and 1024 and be a multiple of 8. Note: Input resolution is not always the same as output resolution due to upscaling from other features."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createlcmgeneration.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createlcmgeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createtexturegeneration.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createtexturegeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createvariationnobg.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createvariationnobg.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createvariationunzoom.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createvariationunzoom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/delete3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/delete3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/get3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/get3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/listelements.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/listelements.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/listplatformmodels.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/listplatformmodels.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/performinpaintinglcm.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/performinpaintinglcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/performinstantrefine.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/performinstantrefine.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/promptimprove.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/promptimprove.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/promptrandom.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/promptrandom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/operations/uploadmodelasset.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/operations/uploadmodelasset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/__init__.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/element_input.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/element_input.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/lcm_generation_style.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/lcm_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/sd_generation_style.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/sd_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/models/shared/sd_versions.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/models/shared/sd_versions.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/prompt.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/prompt.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/sdk.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '5.3.8'
+    sdk_version: str = '5.3.9'
     gen_version: str = '2.314.0'
-    user_agent: str = 'speakeasy-sdk/python 5.3.8 2.314.0 v1.0.0 Leonardo-Ai-SDK'
+    user_agent: str = 'speakeasy-sdk/python 5.3.9 2.314.0 v1.0.0 Leonardo-Ai-SDK'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.8/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-5.3.9/src/leonardoaisdk/variation.py`

 * *Files identical despite different names*

