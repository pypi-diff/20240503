# Comparing `tmp/cryoemservices-0.2.1.tar.gz` & `tmp/cryoemservices-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryoemservices-0.2.1.tar", last modified: Mon Apr  8 10:55:30 2024, max compression
+gzip compressed data, was "cryoemservices-0.2.2.tar", last modified: Fri May  3 09:55:34 2024, max compression
```

## Comparing `cryoemservices-0.2.1.tar` & `cryoemservices-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-08 10:55:30.277920 cryoemservices-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.265920 cryoemservices-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.265920 cryoemservices-0.2.1/src/cryoemservices/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.269920 cryoemservices-0.2.1/src/cryoemservices/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/cli/resubmit_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.269920 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/combine_star_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/combine_star_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/reextract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/src/cryoemservices/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/bfactor_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/cluster_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/cryolo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/ctffind.py
--rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/denoise_iris.py
--rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/extract_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    21270 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/icebreaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/images_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    46671 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/ispyb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/ispyb_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27255 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/motioncorr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/motioncorr_slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/node_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/select_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/select_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22102 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/tomo_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/tomo_align_iris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/src/cryoemservices/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/util/dispatcher_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/util/spa_output_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/util/spa_relion_service_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/src/cryoemservices/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/wrappers/class2d_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/wrappers/class3d_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/wrappers/refine3d_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/src/cryoemservices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-03 09:55:34.161049 cryoemservices-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.149048 cryoemservices-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.149048 cryoemservices-0.2.2/src/cryoemservices/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.153049 cryoemservices-0.2.2/src/cryoemservices/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/cli/resubmit_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.153049 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/combine_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/combine_star_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/reextract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/src/cryoemservices/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/bfactor_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/cluster_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/cryolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/ctffind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/denoise_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/extract_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/icebreaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/images_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46671 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/ispyb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/ispyb_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27301 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/motioncorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/motioncorr_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/node_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21298 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/select_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/select_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22125 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/tomo_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/tomo_align_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/src/cryoemservices/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/dispatcher_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/slurm_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/spa_output_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/spa_relion_service_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/src/cryoemservices/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/wrappers/class2d_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24579 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/wrappers/class3d_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/wrappers/refine3d_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/src/cryoemservices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:55:33.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/top_level.txt
```

### Comparing `cryoemservices-0.2.1/LICENSE` & `cryoemservices-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/PKG-INFO` & `cryoemservices-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoemservices
-Version: 0.2.1
+Version: 0.2.2
 Summary: Services for CryoEM processing
 Author: Diamond Light Source - Data Analysis et al.
 Author-email: dataanalysis@diamond.ac.uk
 License: BSD 3-Clause
 Project-URL: GitHub, https://github.com/DiamondLightSource/cryoem-services
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/cryoem-services/issues
 Keywords: cryoem-services
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gemmi==0.6.5
 Requires-Dist: healpy
-Requires-Dist: htcondor
 Requires-Dist: icebreaker-em
 Requires-Dist: importlib_metadata
 Requires-Dist: ispyb
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: mrcfile
 Requires-Dist: numpy
 Requires-Dist: pillow
```

### Comparing `cryoemservices-0.2.1/README.md` & `cryoemservices-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/setup.cfg` & `cryoemservices-0.2.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cryoemservices
-version = 0.2.1
+version = 0.2.2
 description = Services for CryoEM processing
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Diamond Light Source - Data Analysis et al.
 author_email = dataanalysis@diamond.ac.uk
 license = BSD 3-Clause
 license_files = LICENSE
@@ -23,15 +23,14 @@
 	Bug-Tracker = https://github.com/DiamondLightSource/cryoem-services/issues
 
 [options]
 include_package_data = True
 install_requires = 
 	gemmi ==0.6.5
 	healpy
-	htcondor
 	icebreaker-em
 	importlib_metadata
 	ispyb
 	marshmallow-sqlalchemy
 	mrcfile
 	numpy
 	pillow
@@ -62,28 +61,28 @@
 	mrc_central_slice = cryoemservices.services.images_plugins:mrc_central_slice
 	mrc_to_apng = cryoemservices.services.images_plugins:mrc_to_apng
 workflows.services = 
 	BFactor = cryoemservices.services.bfactor_setup:BFactor
 	ClusterSubmission = cryoemservices.services.cluster_submission:ClusterSubmission
 	CrYOLO = cryoemservices.services.cryolo:CrYOLO
 	CTFFind = cryoemservices.services.ctffind:CTFFind
-	DenoiseIris = cryoemservices.services.denoise_iris:DenoiseIris
+	DenoiseSlurm = cryoemservices.services.denoise_slurm:DenoiseSlurm
 	Extract = cryoemservices.services.extract:Extract
 	ExtractClass = cryoemservices.services.extract_class:ExtractClass
 	IceBreaker = cryoemservices.services.icebreaker:IceBreaker
 	Images = cryoemservices.services.images:Images
 	ISPyB = cryoemservices.services.ispyb:EMISPyB
 	MotionCorr = cryoemservices.services.motioncorr:MotionCorr
 	MotionCorrSlurm = cryoemservices.services.motioncorr_slurm:MotionCorrSlurm
 	NodeCreator = cryoemservices.services.node_creator:NodeCreator
 	PostProcess = cryoemservices.services.postprocess:PostProcess
 	SelectClasses = cryoemservices.services.select_classes:SelectClasses
 	SelectParticles = cryoemservices.services.select_particles:SelectParticles
 	TomoAlign = cryoemservices.services.tomo_align:TomoAlign
-	TomoAlignIris = cryoemservices.services.tomo_align_iris:TomoAlignIris
+	TomoAlignSlurm = cryoemservices.services.tomo_align_slurm:TomoAlignSlurm
 zocalo.services.dispatcher.filters = 
 	ispyb = cryoemservices.util.dispatcher_tools:ispyb_filter
 zocalo.services.dispatcher.ready_for_processing = 
 	ispyb = cryoemservices.util.dispatcher_tools:ready_for_processing
 zocalo.wrappers = 
 	Class2D = cryoemservices.wrappers.class2d_wrapper:Class2DWrapper
 	Class3D = cryoemservices.wrappers.class3d_wrapper:Class3DWrapper
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices/cli/resubmit_wrapper.py` & `cryoemservices-0.2.2/src/cryoemservices/cli/resubmit_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/combine_star_files.py` & `cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/combine_star_files.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/combine_star_job.py` & `cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/combine_star_job.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/reextract.py` & `cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/reextract.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         # Add to output stack
         if len(output_mrc_stack):
             output_mrc_stack = np.append(output_mrc_stack, [particle_subimage], axis=0)
         else:
             output_mrc_stack = np.array([particle_subimage], dtype=np.float32)
 
     # Produce the mrc file of the extracted particles
-    Path(reextract_name).parent.mkdir(exist_ok=True)
+    Path(reextract_name).parent.mkdir(exist_ok=True, parents=True)
     particle_count = np.shape(output_mrc_stack)[0]
     if particle_count > 0:
         with mrcfile.new(str(reextract_name), overwrite=True) as mrc:
             mrc.set_data(output_mrc_stack.astype(np.float32))
             mrc.header.mx = scaled_boxsize
             mrc.header.my = scaled_boxsize
             mrc.header.mz = 1
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/bfactor_setup.py` & `cryoemservices-0.2.2/src/cryoemservices/services/bfactor_setup.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/cluster_submission.py` & `cryoemservices-0.2.2/src/cryoemservices/services/cluster_submission.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/cryolo.py` & `cryoemservices-0.2.2/src/cryoemservices/services/cryolo.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/ctffind.py` & `cryoemservices-0.2.2/src/cryoemservices/services/ctffind.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/extract.py` & `cryoemservices-0.2.2/src/cryoemservices/services/extract.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/images.py` & `cryoemservices-0.2.2/src/cryoemservices/services/images.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/images_plugins.py` & `cryoemservices-0.2.2/src/cryoemservices/services/images_plugins.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/ispyb.py` & `cryoemservices-0.2.2/src/cryoemservices/services/ispyb.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/ispyb_buffer.py` & `cryoemservices-0.2.2/src/cryoemservices/services/ispyb_buffer.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/motioncorr.py` & `cryoemservices-0.2.2/src/cryoemservices/services/motioncorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 import string
 import subprocess
 from collections import ChainMap
 from math import hypot
 from pathlib import Path
-from typing import Optional
+from typing import List, Optional
 
 import plotly.express as px
 import workflows.recipe
 from gemmi import cif
 from pydantic import BaseModel, Field, ValidationError, validator
 from workflows.services.common_service import CommonService
 
@@ -152,21 +152,21 @@
         shift_block = shift_cif.find_block("global_shift")
         x_shifts_str = list(shift_block.find_loop("_rlnMicrographShiftX"))
         y_shifts_str = list(shift_block.find_loop("_rlnMicrographShiftY"))
         for frame in range(len(x_shifts_str)):
             self.x_shift_list.append(float(x_shifts_str[frame]))
             self.y_shift_list.append(float(y_shifts_str[frame]))
 
-    def motioncor2(self, command, mrc_out):
+    def motioncor2(self, command: List[str], mrc_out: Path):
         """Run the MotionCor2 command"""
         result = subprocess.run(command, capture_output=True)
         self.parse_mc2_stdout(result.stdout.decode("utf8", "replace"))
         return result
 
-    def relion_motioncorr(self, command, mrc_out):
+    def relion_motioncorr(self, command: List[str], mrc_out: Path):
         """Run Relion's owm motion correction"""
         result = subprocess.run(command, capture_output=True)
         if Path(mrc_out).with_suffix(".star").exists():
             self.parse_relion_mc_output(Path(mrc_out).with_suffix(".star"))
         else:
             self.log.error(
                 f"Relion output log {Path(mrc_out).with_suffix('.star')} not found"
@@ -317,15 +317,15 @@
                     if type(v) is dict:
                         command.extend(
                             (mc2_flags[k], " ".join(str(_) for _ in v.values()))
                         )
                     else:
                         command.extend((mc2_flags[k], str(v)))
             # Run MotionCor2
-            result = self.motioncor2(command, mc_params.mrc_out)
+            result = self.motioncor2(command, Path(mc_params.mrc_out))
 
             dose_weighted = Path(mc_params.mrc_out).parent / (
                 Path(mc_params.mrc_out).stem + "_DW.mrc"
             )
             if dose_weighted.is_file():
                 mc_params.mrc_out = str(dose_weighted)
         else:
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/motioncorr_slurm.py` & `cryoemservices-0.2.2/src/cryoemservices/util/slurm_submission.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,323 +1,288 @@
 from __future__ import annotations
 
 import json
 import os
-import string
 import subprocess
 import time
-from collections import ChainMap
 from pathlib import Path
 
 import yaml
-from workflows.services.common_service import CommonService
 
-from cryoemservices.services.motioncorr import MotionCorr
-
-"""
-This service submits motion correction jobs to a slurm cluster
+""""
+This service submits jobs to a slurm cluster
 To do this it needs environment variables set for the following:
-    MOTIONCOR2_SIF: singularity image of MotionCor2
     SLURM_RESTAPI_CONFIG: configuration yaml file for the slurm cluster
 
 The configuration has the following format:
     plugin: slurm
     url: <url>:<port>
     user_token: <file with restapi token>
     user: <username>
     user_home: <home directory>
     api_version: v0.0.38 or v0.0.40
     partition: <optional slurm partition>
     partition_preference: <optional slurm preferences>
-    clusters: <optional slurm clusters>
+    cluster: <optional slurm clusters>
     required_directories: [<list of directories to bind for singularity>]
 """
 
 slurm_json_job_template = {
     "v0.0.38": {
-        "name": "MotionCorr",
         "nodes": 1,
         "tasks": 1,
-        "cpus_per_task": 1,
-        "gpus": 1,
-        "memory_per_gpu": 12000,
         "time_limit": "1:00:00",
     },
     "v0.0.40": {
-        "name": "MotionCorr",
         "minimum_nodes": 1,
         "maximum_nodes": 1,
         "tasks": 1,
-        "cpus_per_task": 1,
-        "tres_per_task": "gres/gpu:1",
         "memory_per_node": {
             "number": 12000,
             "set": True,
             "infinite": False,
         },
         "time_limit": {
             "number": 3600,
             "set": True,
             "infinite": False,
         },
     },
 }
-slurm_script_template = (
+
+# Templates for running a command using singularity or by with a module/executable
+singularity_script_template = (
     "#!/bin/bash\n"
-    "echo \"$(date '+%Y-%m-%d %H:%M:%S.%3N'): running MotionCor2\"\n"
+    "echo \"$(date '+%Y-%m-%d %H:%M:%S.%3N'): running slurm job\"\n"
     "mkdir /tmp/tmp_$SLURM_JOB_ID\n"
     "export APPTAINER_CACHEDIR=/tmp/tmp_$SLURM_JOB_ID\n"
     "export APPTAINER_TMPDIR=/tmp/tmp_$SLURM_JOB_ID\n"
-    "singularity exec --nv --bind /lib64,/tmp/tmp_$SLURM_JOB_ID:/tmp"
+)
+module_script_template = (
+    "#!/bin/bash\n"
+    "echo \"$(date '+%Y-%m-%d %H:%M:%S.%3N'): running slurm job\"\n"
+    "source /etc/profile.d/modules.sh\n"
 )
 slurm_tmp_cleanup = "\nrm -rf /tmp/tmp_$SLURM_JOB_ID"
 
 
-class ChainMapWithReplacement(ChainMap):
-    def __init__(self, *maps, substitutions=None) -> None:
-        super().__init__(*maps)
-        self._substitutions = substitutions
-
-    def __getitem__(self, k):
-        v = super().__getitem__(k)
-        if self._substitutions and isinstance(v, str) and "$" in v:
-            template = string.Template(v)
-            return template.substitute(**self._substitutions)
-        return v
-
-
-class MotionCorrSlurm(MotionCorr, CommonService):
-    """
-    A service for submitting MotionCor2 jobs to slurm via a RestAPI
-    """
-
-    # Logger name
-    _logger_name = "cryoemservices.services.motioncorr_slurm"
-
-    def parse_mc_slurm_output(self, mc_output_file):
-        """
-        Read the output logs of MotionCorr to determine
-        the movement of each frame
-        """
-        with open(mc_output_file, "r") as mc_file:
-            lines = mc_file.readlines()
-            frames_line = False
-            for line in lines:
-                # Frame reading in MotionCorr 1.4.0
-                if line.startswith("...... Frame"):
-                    line_split = line.split()
-                    self.x_shift_list.append(float(line_split[-2]))
-                    self.y_shift_list.append(float(line_split[-1]))
-
-                # Alternative frame reading for MotionCorr 1.6.3
-                if not line:
-                    frames_line = False
-                if frames_line:
-                    line_split = line.split()
-                    self.x_shift_list.append(float(line_split[1]))
-                    self.y_shift_list.append(float(line_split[2]))
-                if "x Shift" in line:
-                    frames_line = True
-
-    def motioncor2(self, command: list, mrc_out: Path):
-        """Submit MotionCor2 jobs to the slurm cluster via the RestAPI"""
-        try:
-            # Get the configuration and token for the restAPI
-            with open(os.environ["SLURM_RESTAPI_CONFIG"], "r") as f:
-                slurm_rest = yaml.safe_load(f)
-            user = slurm_rest["user"]
-            user_home = slurm_rest["user_home"]
-            with open(slurm_rest["user_token"], "r") as f:
-                slurm_token = f.read().strip()
-        except (KeyError, FileNotFoundError):
-            self.log.error("Unable to load slurm restAPI config file and token")
-            return subprocess.CompletedProcess(
-                args="",
-                returncode=1,
-                stdout="".encode("utf8"),
-                stderr="No restAPI config or token".encode("utf8"),
-            )
+def slurm_submission(
+    log,
+    job_name: str,
+    command: list,
+    project_dir: Path,
+    output_file: Path,
+    cpus: int,
+    use_gpu: bool,
+    use_singularity: bool,
+    cif_name: str = "",
+    script_extras: str = "",
+    external_filesystem: bool = False,
+):
+    """Submit jobs to a slurm cluster via the RestAPI"""
+    try:
+        # Get the configuration and token for the restAPI
+        with open(os.environ["SLURM_RESTAPI_CONFIG"], "r") as f:
+            slurm_rest = yaml.safe_load(f)
+        user = slurm_rest["user"]
+        user_home = slurm_rest["user_home"]
+        with open(slurm_rest["user_token"], "r") as f:
+            slurm_token = f.read().strip()
+    except (KeyError, FileNotFoundError):
+        log.error("Unable to load slurm restAPI config file and token")
+        return subprocess.CompletedProcess(
+            args="",
+            returncode=1,
+            stdout="".encode("utf8"),
+            stderr="No restAPI config or token".encode("utf8"),
+        )
 
-        # Check the API version is one this service has been tested with
-        api_version = slurm_rest["api_version"]
-        print(api_version)
-        if api_version not in ["v0.0.38", "v0.0.40"]:
-            return subprocess.CompletedProcess(
-                args="",
-                returncode=1,
-                stdout="".encode("utf8"),
-                stderr=f"Unsupported API version {api_version}".encode("utf8"),
-            )
+    # Check the API version is one this service has been tested with
+    api_version = slurm_rest["api_version"]
+    if api_version not in ["v0.0.38", "v0.0.40"]:
+        return subprocess.CompletedProcess(
+            args="",
+            returncode=1,
+            stdout="".encode("utf8"),
+            stderr=f"Unsupported API version {api_version}".encode("utf8"),
+        )
 
-        # Construct the json for submission
-        mc_output_file = f"{mrc_out}.out"
-        mc_error_file = f"{mrc_out}.err"
-        submission_file = f"{mrc_out}.json"
-        slurm_config = {
-            "standard_output": mc_output_file,
-            "standard_error": mc_error_file,
-            "current_working_directory": str(Path(mrc_out).parent),
-        }
+    # Construct the json for submission
+    slurm_output_file = f"{output_file}.out"
+    slurm_error_file = f"{output_file}.err"
+    submission_file = f"{output_file}.json"
+    slurm_config = {
+        "standard_output": slurm_output_file,
+        "standard_error": slurm_error_file,
+        "current_working_directory": str(project_dir),
+    }
+    if api_version == "v0.0.38":
+        slurm_config["environment"] = {"USER": user, "HOME": user_home}
+    else:
+        slurm_config["environment"] = [f"USER: {user}", f"HOME: {user_home}"]
+
+    # Add slurm partition and cluster preferences if given
+    if slurm_rest.get("partition"):
+        slurm_config["partition"] = slurm_rest["partition"]
+    if slurm_rest.get("partition_preference"):
+        slurm_config["prefer"] = slurm_rest["partition_preference"]
+    if slurm_rest.get("cluster"):
+        slurm_config["cluster"] = slurm_rest["cluster"]
+
+    # Combine this with the template for the given API version
+    slurm_json_job = dict(slurm_json_job_template[api_version], **slurm_config)
+    slurm_json_job["name"] = job_name
+    slurm_json_job["cpus_per_task"] = cpus
+    if use_gpu:
         if api_version == "v0.0.38":
-            slurm_config["environment"] = {"USER": user, "HOME": user_home}
+            slurm_json_job["gpus"] = 1
+            slurm_json_job["memory_per_gpu"] = 12000
         else:
-            slurm_config["environment"] = [f"USER: {user}", f"HOME: {user_home}"]
-
-        # Add slurm partition and cluster preferences if given
-        if slurm_rest.get("partition"):
-            slurm_config["partition"] = slurm_rest["partition"]
-        if slurm_rest.get("partition_preference"):
-            slurm_config["prefer"] = slurm_rest["partition_preference"]
-        if slurm_rest.get("clusters"):
-            slurm_config["clusters"] = slurm_rest["clusters"]
-        # Combine this with the template for the given API version
-        slurm_json_job = dict(slurm_json_job_template[api_version], **slurm_config)
+            slurm_json_job["tres_per_task"] = "gres/gpu:1"
+    elif api_version == "v0.0.38":
+        slurm_json_job["memory_per_cpu"] = 1000
 
-        # Make the script command and save the submission json
+    # Construct the job command and save the job script
+    if use_singularity:
         if slurm_rest.get("required_directories"):
             binding_dirs = "," + ",".join(slurm_rest["required_directories"])
         else:
             binding_dirs = ""
         job_command = (
-            slurm_script_template
-            + f"{binding_dirs} --home {user_home} {os.environ['MOTIONCOR2_SIF']} "
+            singularity_script_template
+            + script_extras
+            + "\n"
+            + "singularity exec --nv --bind /lib64,/tmp/tmp_$SLURM_JOB_ID:/tmp"
+            + f"{binding_dirs} --home {user_home} {cif_name} "
             + " ".join(command)
             + slurm_tmp_cleanup
         )
-        slurm_json = {"job": slurm_json_job, "script": job_command}
-        with open(submission_file, "w") as f:
-            json.dump(slurm_json, f)
-
-        # Command to submit jobs to the restAPI
-        slurm_submit_command = (
-            f'curl -H "X-SLURM-USER-NAME:{user}" -H "X-SLURM-USER-TOKEN:{slurm_token}" '
-            '-H "Content-Type: application/json" -X POST '
-            f'{slurm_rest["url"]}/slurm/{slurm_rest["api_version"]}/job/submit '
-            f"-d @{submission_file}"
+    else:
+        job_command = module_script_template + script_extras + "\n" + " ".join(command)
+    slurm_json = {"job": slurm_json_job, "script": job_command}
+    with open(submission_file, "w") as f:
+        json.dump(slurm_json, f)
+
+    # Command to submit jobs to the restAPI
+    slurm_submit_command = (
+        f'curl -H "X-SLURM-USER-NAME:{user}" -H "X-SLURM-USER-TOKEN:{slurm_token}" '
+        '-H "Content-Type: application/json" -X POST '
+        f'{slurm_rest["url"]}/slurm/{slurm_rest["api_version"]}/job/submit '
+        f"-d @{submission_file}"
+    )
+    slurm_submission_json = subprocess.run(
+        slurm_submit_command, capture_output=True, shell=True
+    )
+    try:
+        # Extract the job id from the submission response to use in the next query
+        slurm_response = slurm_submission_json.stdout.decode("utf8", "replace")
+        slurm_response_json = json.loads(slurm_response)
+        job_id = slurm_response_json["job_id"]
+    except (json.JSONDecodeError, KeyError):
+        log.error(
+            f"Unable to submit job to {slurm_rest['url']}. The restAPI returned "
+            f"{slurm_submission_json.stdout.decode('utf8', 'replace')}"
+        )
+        return subprocess.CompletedProcess(
+            args="",
+            returncode=1,
+            stdout=slurm_submission_json.stdout,
+            stderr=slurm_submission_json.stderr,
         )
-        slurm_submission_json = subprocess.run(
-            slurm_submit_command, capture_output=True, shell=True
+    log.info(f"Submitted job {job_id} for {job_name} to slurm. Waiting...")
+    if slurm_response_json.get("warnings") and slurm_response_json["warnings"]:
+        log.warning(f"Slurm reported these warnings: {slurm_response_json['warnings']}")
+    if slurm_response_json.get("errors") and slurm_response_json["errors"]:
+        log.warning(f"Slurm reported these errors: {slurm_response_json['errors']}")
+
+    # Command to get the status of the submitted job from the restAPI
+    slurm_status_command = (
+        f'curl -H "X-SLURM-USER-NAME:{user}" -H "X-SLURM-USER-TOKEN:{slurm_token}" '
+        '-H "Content-Type: application/json" -X GET '
+        f'{slurm_rest["url"]}/slurm/{slurm_rest["api_version"]}/job/{job_id}'
+    )
+    slurm_job_state = "PENDING"
+
+    # Wait until the job has a status indicating it has finished
+    loop_counter = 0
+    while slurm_job_state in (
+        "PENDING",
+        "CONFIGURING",
+        "RUNNING",
+        "COMPLETING",
+    ):
+        if loop_counter < 5:
+            time.sleep(5)
+        else:
+            time.sleep(30)
+        loop_counter += 1
+
+        # Call the restAPI to find out the job state
+        slurm_status_json = subprocess.run(
+            slurm_status_command, capture_output=True, shell=True
         )
         try:
-            # Extract the job id from the submission response to use in the next query
-            slurm_response = slurm_submission_json.stdout.decode("utf8", "replace")
-            slurm_response_json = json.loads(slurm_response)
-            job_id = slurm_response_json["job_id"]
+            slurm_response = slurm_status_json.stdout.decode("utf8", "replace")
+            slurm_job_state = json.loads(slurm_response)["jobs"][0]["job_state"]
+            if api_version == "v0.0.40":
+                slurm_job_state = slurm_job_state[0]
         except (json.JSONDecodeError, KeyError):
-            self.log.error(
-                f"Unable to submit job to {slurm_rest['url']}. The restAPI returned "
-                f"{slurm_submission_json.stdout.decode('utf8', 'replace')}"
+            print(slurm_status_command)
+            log.error(
+                f"Unable to get status for job {job_id}. The restAPI returned "
+                f"{slurm_status_json.stdout.decode('utf8', 'replace')}"
             )
             return subprocess.CompletedProcess(
                 args="",
                 returncode=1,
-                stdout=slurm_submission_json.stdout,
-                stderr=slurm_submission_json.stderr,
+                stdout=slurm_status_json.stdout,
+                stderr=slurm_status_json.stderr,
             )
-        self.log.info(f"Submitted MotionCorr job {job_id} to slurm. Waiting...")
-        if slurm_response_json.get("warnings") and slurm_response_json["warnings"]:
-            self.log.warning(
-                f"Slurm reported these warnings: {slurm_response_json['warnings']}"
-            )
-        if slurm_response_json.get("errors") and slurm_response_json["errors"]:
-            self.log.warning(
-                f"Slurm reported these errors: {slurm_response_json['errors']}"
-            )
-
-        # Command to get the status of the submitted job from the restAPI
-        slurm_status_command = (
-            f'curl -H "X-SLURM-USER-NAME:{user}" -H "X-SLURM-USER-TOKEN:{slurm_token}" '
-            '-H "Content-Type: application/json" -X GET '
-            f'{slurm_rest["url"]}/slurm/{slurm_rest["api_version"]}/job/{job_id}'
-        )
-        slurm_job_state = "PENDING"
 
-        # Wait until the job has a status indicating it has finished
-        loop_counter = 0
-        while slurm_job_state in (
-            "PENDING",
-            "CONFIGURING",
-            "RUNNING",
-            "COMPLETING",
-        ):
-            if loop_counter < 5:
-                time.sleep(5)
-            else:
-                time.sleep(30)
-            loop_counter += 1
-
-            # Call the restAPI to find out the job state
-            slurm_status_json = subprocess.run(
-                slurm_status_command, capture_output=True, shell=True
+        if loop_counter >= 60:
+            slurm_cancel_command = (
+                f'curl -H "X-SLURM-USER-NAME:{user}" '
+                f'-H "X-SLURM-USER-TOKEN:{slurm_token}" '
+                '-H "Content-Type: application/json" -X DELETE '
+                f'{slurm_rest["url"]}/slurm/{slurm_rest["api_version"]}/job/{job_id}'
+            )
+            subprocess.run(slurm_cancel_command, capture_output=True, shell=True)
+            log.error(f"Timeout running {job_name}")
+            return subprocess.CompletedProcess(
+                args="",
+                returncode=1,
+                stdout="".encode("utf8"),
+                stderr=f"Timeout running {job_name}".encode("utf8"),
             )
-            try:
-                slurm_response = slurm_status_json.stdout.decode("utf8", "replace")
-                slurm_job_state = json.loads(slurm_response)["jobs"][0]["job_state"]
-                if api_version == "v0.0.40":
-                    slurm_job_state = slurm_job_state[0]
-            except (json.JSONDecodeError, IndexError, KeyError):
-                print(slurm_status_command)
-                self.log.error(
-                    f"Unable to get status for job {job_id}. The restAPI returned "
-                    f"{slurm_status_json.stdout.decode('utf8', 'replace')}"
-                )
-                return subprocess.CompletedProcess(
-                    args="",
-                    returncode=1,
-                    stdout=slurm_status_json.stdout,
-                    stderr=slurm_status_json.stderr,
-                )
-
-            if loop_counter >= 60:
-                slurm_cancel_command = (
-                    f'curl -H "X-SLURM-USER-NAME:{user}" '
-                    f'-H "X-SLURM-USER-TOKEN:{slurm_token}" '
-                    '-H "Content-Type: application/json" -X DELETE '
-                    f'{slurm_rest["url"]}/slurm/{slurm_rest["api_version"]}/job/{job_id}'
-                )
-                subprocess.run(slurm_cancel_command, capture_output=True, shell=True)
-                self.log.error("Timeout running motion correction")
-                return subprocess.CompletedProcess(
-                    args="",
-                    returncode=1,
-                    stdout="".encode("utf8"),
-                    stderr="Timeout running motion correction".encode("utf8"),
-                )
 
-        # Read in the MotionCor output then clean up the files
-        self.log.info(f"Job {job_id} has finished!")
+    # Read in the output
+    log.info(f"Job {job_id} has finished!")
+    if not external_filesystem:
         try:
-            self.parse_mc_slurm_output(mc_output_file)
-            with open(mc_output_file, "r") as mc_stdout:
-                stdout = mc_stdout.read()
-            with open(mc_error_file, "r") as mc_stderr:
-                stderr = mc_stderr.read()
+            with open(slurm_output_file, "r") as slurm_stdout:
+                stdout = slurm_stdout.read()
+            with open(slurm_error_file, "r") as slurm_stderr:
+                stderr = slurm_stderr.read()
         except FileNotFoundError:
-            self.log.error(f"MotionCor output file {mc_output_file} not found")
+            log.error(f"Output file {slurm_output_file} not found")
             stdout = ""
-            stderr = f"Reading MotionCor output file {mc_output_file} failed"
-            slurm_job_state = "FAILED"
-
-        if self.x_shift_list and self.y_shift_list:
-            Path(mc_output_file).unlink()
-            Path(mc_error_file).unlink()
-            Path(submission_file).unlink()
-        else:
-            self.log.error(f"Reading shifts from {mc_output_file} failed")
+            stderr = f"Reading output file {slurm_error_file} failed"
             slurm_job_state = "FAILED"
-
-        if slurm_job_state == "COMPLETED":
-            return subprocess.CompletedProcess(
-                args="",
-                returncode=0,
-                stdout=stdout.encode("utf8"),
-                stderr=stderr.encode("utf8"),
-            )
-        else:
-            self.x_shift_list = []
-            self.y_shift_list = []
-            return subprocess.CompletedProcess(
-                args="",
-                returncode=1,
-                stdout=stdout.encode("utf8"),
-                stderr=stderr.encode("utf8"),
-            )
+    else:
+        stdout = ""
+        stderr = ""
+
+    # Read in the output then clean up the files
+    if slurm_job_state == "COMPLETED":
+        return subprocess.CompletedProcess(
+            args="",
+            returncode=0,
+            stdout=stdout.encode("utf8"),
+            stderr=stderr.encode("utf8"),
+        )
+    else:
+        return subprocess.CompletedProcess(
+            args="",
+            returncode=1,
+            stdout=stdout.encode("utf8"),
+            stderr=stderr.encode("utf8"),
+        )
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/node_creator.py` & `cryoemservices-0.2.2/src/cryoemservices/services/node_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import datetime
 import json
 import os
 import re
+import time
 from pathlib import Path
 from typing import Optional
 
 import workflows.recipe
 from pipeliner.api.api_utils import (
     edit_jobstar,
     job_default_parameters_dict,
@@ -134,14 +135,15 @@
     output_file: str = Field(..., min_length=1)
     relion_options: RelionServiceOptions
     command: str
     stdout: str
     stderr: str
     success: bool = True
     results: Optional[dict] = None
+    alias: Optional[str] = None
 
 
 class NodeCreator(CommonService):
     """
     A service for setting up pipeliner jobs
     """
 
@@ -366,20 +368,42 @@
                 for results_obj in results_files:
                     results_obj.unlink()
 
                 results_displays = pipeliner_job.create_results_display()
                 for results_obj in results_displays:
                     results_obj.write_displayobj_file(outdir=str(job_dir))
 
+        # Check the lock status
+        if (
+            Path(project_dir / ".relion_lock").is_dir()
+            or Path(job_dir / ".relion_lock").is_dir()
+        ):
+            self.log.warning("WARNING: Relion lock found")
+            time.sleep(5)
+            try:
+                Path(project_dir / ".relion_lock").rmdir()
+                self.log.warning("Relion project lock has been removed")
+            except FileNotFoundError:
+                self.log.warning("No project lock found to remove")
+            try:
+                Path(job_dir / ".relion_lock").rmdir()
+                self.log.warning("Relion job lock has been removed")
+            except FileNotFoundError:
+                self.log.warning("No job lock found to remove")
+
+        if job_info.alias:
+            (job_dir.parent / job_info.alias).unlink(missing_ok=True)
+
         # Create the node and default_pipeline.star files in the project directory
         with ProjectGraph(read_only=False) as project:
             process = project.add_job(
                 pipeliner_job,
                 as_status=("Succeeded" if job_info.success else "Failed"),
                 do_overwrite=True,
+                alias=job_info.alias,
             )
             # Add the job commands to the process .CCPEM_pipeliner_jobinfo file
             if not (job_dir / ".CCPEM_pipeliner_jobinfo").exists():
                 process.update_jobinfo_file(action="Run", command_list=relion_commands)
             # Generate the default_pipeline.star file
             project.check_process_completion()
             # Copy the default_pipeline.star file
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/postprocess.py` & `cryoemservices-0.2.2/src/cryoemservices/services/postprocess.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/select_classes.py` & `cryoemservices-0.2.2/src/cryoemservices/services/select_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,14 +329,15 @@
                 "command": (
                     "combine_star_files "
                     + " ".join([str(i) for i in files_to_combine])
                     + f" --output_dir {combine_star_dir}"
                 ),
                 "stdout": "",
                 "stderr": "",
+                "alias": "Best_particles",
             }
 
             # Call the combining function and redirect prints to an io object
             combine_result = io.StringIO()
             with redirect_stdout(combine_result):
                 try:
                     combine_star_files(files_to_combine, combine_star_dir)
@@ -446,14 +447,15 @@
             "command": (
                 f"combine_star_files {combine_star_dir}/particles_all.star "
                 f"--output_dir {combine_star_dir} "
                 f"--split --split_size {next_batch_size}"
             ),
             "stdout": "",
             "stderr": "",
+            "alias": "Best_particles",
         }
 
         # Call the combining function and redirect prints to an io object
         split_result = io.StringIO()
         with redirect_stdout(split_result):
             try:
                 split_star_file(
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/select_particles.py` & `cryoemservices-0.2.2/src/cryoemservices/services/select_particles.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/services/tomo_align.py` & `cryoemservices-0.2.2/src/cryoemservices/services/tomo_align.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 
 class TomoParameters(BaseModel):
     stack_file: str = Field(..., min_length=1)
     path_pattern: str = None
     input_file_list: str = None
     position: Optional[str] = None
-    aretomo_output_file: Optional[str] = None
     vol_z: int = 1200
     align: Optional[int] = None
     out_bin: int = 4
     tilt_axis: Optional[float] = None
     tilt_cor: int = 1
     flip_int: Optional[int] = None
     flip_vol: int = 1
@@ -99,14 +98,15 @@
     xy_proj_file: str | None = None
     xz_proj_file: str | None = None
     central_slice_file: str | None = None
     tomogram_movie_file: str | None = None
     newstack_path: str | None = None
     alignment_output_dir: str | None = None
     stack_name: str | None = None
+    aretomo_output_path: str | None = None
     alignment_quality: float | None = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.refined_tilts = []
         self.rot_centre_z_list = []
 
@@ -144,18 +144,16 @@
                 tomo_aln_file = aln_file
 
         with open(tomo_aln_file) as f:
             lines = f.readlines()
             for line in lines:
                 if not line.startswith("#"):
                     line_split = line.split()
-                    if self.rot is None:
-                        self.rot = float(line_split[1])
-                    if self.mag is None:
-                        self.mag = float(line_split[2])
+                    self.rot = float(line_split[1])
+                    self.mag = float(line_split[2])
                     x_shift.append(float(line_split[3]))
                     y_shift.append(float(line_split[4]))
                     self.refined_tilts.append(float(line_split[9]))
         fig = px.scatter(x=x_shift, y=y_shift)
         fig.write_json(self.plot_path)
         return tomo_aln_file  # not needed anywhere atm
 
@@ -219,14 +217,15 @@
                     if "." in part:
                         input_file_list.append([str(item), part])
             tomo_params.input_file_list = input_file_list
 
         self.log.info(f"Input list {tomo_params.input_file_list}")
         tomo_params.input_file_list.sort(key=_tilt)
 
+        # Find all the tilt angles and remove duplicates
         tilt_dict: dict = {}
         for tilt in tomo_params.input_file_list:
             if not Path(tilt[0]).is_file():
                 self.log.warning(f"File not found {tilt[0]}")
                 rw.transport.nack(header)
             if tilt[1] not in tilt_dict:
                 tilt_dict[tilt[1]] = []
@@ -234,28 +233,27 @@
 
         values_to_remove = []
         for item in tilt_dict:
             values = tilt_dict[item]
             if len(values) > 1:
                 # sort by age and remove oldest ones
                 values.sort(key=os.path.getctime)
-                values_to_remove = values[1:]
+                values_to_remove.append(values[1:])
 
         for tilt in tomo_params.input_file_list:
             if tilt[0] in values_to_remove:
                 index = tomo_params.input_file_list.index(tilt)
                 self.log.warning(f"Removing: {values_to_remove}")
                 tomo_params.input_file_list.remove(tomo_params.input_file_list[index])
 
         self.alignment_output_dir = str(Path(tomo_params.stack_file).parent)
         self.stack_name = str(Path(tomo_params.stack_file).stem)
 
-        tomo_params.aretomo_output_file = self.stack_name + "_aretomo.mrc"
         self.aretomo_output_path = (
-            self.alignment_output_dir + "/" + tomo_params.aretomo_output_file
+            self.alignment_output_dir + "/" + self.stack_name + "_aretomo.mrc"
         )
         self.plot_file = self.stack_name + "_xy_shift_plot.json"
         self.plot_path = self.alignment_output_dir + "/" + self.plot_file
         self.dark_images_file = self.stack_name + "_DarkImgs.txt"
         self.xy_proj_file = self.stack_name + "_aretomo_projXY.jpeg"
         self.xz_proj_file = self.stack_name + "_aretomo_projXZ.jpeg"
         self.central_slice_file = self.stack_name + "_aretomo_thumbnail.jpeg"
@@ -341,15 +339,19 @@
             pix_spacing = None
         # Forward results to ispyb
 
         # Tomogram (one per-tilt-series)
         ispyb_command_list = [
             {
                 "ispyb_command": "insert_tomogram",
-                "volume_file": tomo_params.aretomo_output_file,
+                "volume_file": str(
+                    Path(self.aretomo_output_path).relative_to(
+                        self.alignment_output_dir
+                    )
+                ),
                 "stack_file": tomo_params.stack_file,
                 "size_x": None,  # volume image size, pix
                 "size_y": None,
                 "size_z": None,
                 "pixel_spacing": pix_spacing,
                 "tilt_angle_offset": str(self.tilt_offset),
                 "z_shift": self.rot_centre_z,
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices/util/dispatcher_tools.py` & `cryoemservices-0.2.2/src/cryoemservices/util/dispatcher_tools.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/util/spa_output_files.py` & `cryoemservices-0.2.2/src/cryoemservices/util/spa_output_files.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/util/spa_relion_service_options.py` & `cryoemservices-0.2.2/src/cryoemservices/util/spa_relion_service_options.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/wrappers/class2d_wrapper.py` & `cryoemservices-0.2.2/src/cryoemservices/wrappers/class2d_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.1/src/cryoemservices/wrappers/class3d_wrapper.py` & `cryoemservices-0.2.2/src/cryoemservices/wrappers/class3d_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,14 +506,15 @@
         )
         classes_block = class_star_file.find_block("model_classes")
         classes_loop = classes_block.find_loop("_rlnReferenceImage").get_loop()
 
         best_class = 0
         best_class_resolution = 100
         best_class_completeness = 0
+        best_class_particles = 0
 
         for class_id in range(class3d_params.class3d_nr_classes):
             # Add an ispyb insert for each class
             class_ispyb_parameters = {
                 "ispyb_command": "buffer",
                 "buffer_lookup": {
                     "particle_classification_group_id": class3d_params.class3d_grp_uuid
@@ -555,20 +556,26 @@
                 class_ispyb_parameters[
                     "overall_fourier_completeness"
                 ] = fourier_completeness
             else:
                 class_ispyb_parameters["overall_fourier_completeness"] = 0.0
 
             # Compare this class to the previous best class
-            if class_ispyb_parameters["estimated_resolution"] < best_class_resolution:
+            if class_ispyb_parameters[
+                "estimated_resolution"
+            ] < best_class_resolution or (
+                class_ispyb_parameters["estimated_resolution"] == best_class_resolution
+                and class_ispyb_parameters["particles_per_class"] > best_class_particles
+            ):
                 best_class = class_id + 1
                 best_class_resolution = class_ispyb_parameters["estimated_resolution"]
                 best_class_completeness = class_ispyb_parameters[
                     "overall_fourier_completeness"
                 ]
+                best_class_particles = class_ispyb_parameters["particles_per_class"]
 
             # Add the ispyb command to the command list
             ispyb_parameters.append(class_ispyb_parameters)
 
         # Add on the initial model insert before sending
         if class3d_params.do_initial_model:
             ispyb_parameters.extend(initial_model_ispyb_parameters)
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices/wrappers/refine3d_wrapper.py` & `cryoemservices-0.2.2/src/cryoemservices/wrappers/refine3d_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,27 +43,27 @@
     mpi_run_command: str = "srun -n 5"
     dont_correct_greyscale: bool = True
     initial_lowpass: float = 20.0
     dont_combine_weights_via_disc: bool = True
     preread_images: bool = True
     scratch_dir: Optional[str] = None
     nr_pool: int = 10
-    pad: int = 1
+    pad: int = 2
     do_ctf: bool = True
     ctf_intact_first_peak: bool = False
     flatten_solvent: bool = True
     do_zero_mask: bool = True
     oversampling: int = 1
     healpix_order: int = 2
     local_healpix_order: int = 4
     low_resol_join_halves: float = 40
     offset_range: float = 5
     offset_step: float = 4
-    ignore_angles: bool = True
-    resol_angles: bool = True
+    ignore_angles: bool = False
+    resol_angles: bool = False
     symmetry: str = "C1"
     do_norm: bool = True
     do_scale: bool = True
     threads: int = 8
     gpus: str = "0:1:2:3"
     relion_options: RelionServiceOptions
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices.egg-info/PKG-INFO` & `cryoemservices-0.2.2/src/cryoemservices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoemservices
-Version: 0.2.1
+Version: 0.2.2
 Summary: Services for CryoEM processing
 Author: Diamond Light Source - Data Analysis et al.
 Author-email: dataanalysis@diamond.ac.uk
 License: BSD 3-Clause
 Project-URL: GitHub, https://github.com/DiamondLightSource/cryoem-services
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/cryoem-services/issues
 Keywords: cryoem-services
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gemmi==0.6.5
 Requires-Dist: healpy
-Requires-Dist: htcondor
 Requires-Dist: icebreaker-em
 Requires-Dist: importlib_metadata
 Requires-Dist: ispyb
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: mrcfile
 Requires-Dist: numpy
 Requires-Dist: pillow
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices.egg-info/SOURCES.txt` & `cryoemservices-0.2.2/src/cryoemservices.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,31 +18,32 @@
 src/cryoemservices/pipeliner_plugins/combine_star_job.py
 src/cryoemservices/pipeliner_plugins/reextract.py
 src/cryoemservices/services/__init__.py
 src/cryoemservices/services/bfactor_setup.py
 src/cryoemservices/services/cluster_submission.py
 src/cryoemservices/services/cryolo.py
 src/cryoemservices/services/ctffind.py
-src/cryoemservices/services/denoise_iris.py
+src/cryoemservices/services/denoise_slurm.py
 src/cryoemservices/services/extract.py
 src/cryoemservices/services/extract_class.py
 src/cryoemservices/services/icebreaker.py
 src/cryoemservices/services/images.py
 src/cryoemservices/services/images_plugins.py
 src/cryoemservices/services/ispyb.py
 src/cryoemservices/services/ispyb_buffer.py
 src/cryoemservices/services/motioncorr.py
 src/cryoemservices/services/motioncorr_slurm.py
 src/cryoemservices/services/node_creator.py
 src/cryoemservices/services/postprocess.py
 src/cryoemservices/services/select_classes.py
 src/cryoemservices/services/select_particles.py
 src/cryoemservices/services/tomo_align.py
-src/cryoemservices/services/tomo_align_iris.py
+src/cryoemservices/services/tomo_align_slurm.py
 src/cryoemservices/util/__init__.py
 src/cryoemservices/util/dispatcher_tools.py
+src/cryoemservices/util/slurm_submission.py
 src/cryoemservices/util/spa_output_files.py
 src/cryoemservices/util/spa_relion_service_options.py
 src/cryoemservices/wrappers/__init__.py
 src/cryoemservices/wrappers/class2d_wrapper.py
 src/cryoemservices/wrappers/class3d_wrapper.py
 src/cryoemservices/wrappers/refine3d_wrapper.py
```

### Comparing `cryoemservices-0.2.1/src/cryoemservices.egg-info/entry_points.txt` & `cryoemservices-0.2.2/src/cryoemservices.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 picked_particles = cryoemservices.services.images_plugins:picked_particles
 
 [workflows.services]
 BFactor = cryoemservices.services.bfactor_setup:BFactor
 CTFFind = cryoemservices.services.ctffind:CTFFind
 ClusterSubmission = cryoemservices.services.cluster_submission:ClusterSubmission
 CrYOLO = cryoemservices.services.cryolo:CrYOLO
-DenoiseIris = cryoemservices.services.denoise_iris:DenoiseIris
+DenoiseSlurm = cryoemservices.services.denoise_slurm:DenoiseSlurm
 Extract = cryoemservices.services.extract:Extract
 ExtractClass = cryoemservices.services.extract_class:ExtractClass
 ISPyB = cryoemservices.services.ispyb:EMISPyB
 IceBreaker = cryoemservices.services.icebreaker:IceBreaker
 Images = cryoemservices.services.images:Images
 MotionCorr = cryoemservices.services.motioncorr:MotionCorr
 MotionCorrSlurm = cryoemservices.services.motioncorr_slurm:MotionCorrSlurm
 NodeCreator = cryoemservices.services.node_creator:NodeCreator
 PostProcess = cryoemservices.services.postprocess:PostProcess
 SelectClasses = cryoemservices.services.select_classes:SelectClasses
 SelectParticles = cryoemservices.services.select_particles:SelectParticles
 TomoAlign = cryoemservices.services.tomo_align:TomoAlign
-TomoAlignIris = cryoemservices.services.tomo_align_iris:TomoAlignIris
+TomoAlignSlurm = cryoemservices.services.tomo_align_slurm:TomoAlignSlurm
 
 [zocalo.services.dispatcher.filters]
 ispyb = cryoemservices.util.dispatcher_tools:ispyb_filter
 
 [zocalo.services.dispatcher.ready_for_processing]
 ispyb = cryoemservices.util.dispatcher_tools:ready_for_processing
```

