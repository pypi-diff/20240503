# Comparing `tmp/cyto-dl-0.1.5.tar.gz` & `tmp/cyto-dl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyto-dl-0.1.5.tar", last modified: Mon Apr  1 23:14:26 2024, max compression
+gzip compressed data, was "cyto-dl-0.1.6.tar", last modified: Fri May  3 16:17:38 2024, max compression
```

## Comparing `cyto-dl-0.1.5.tar` & `cyto-dl-0.1.6.tar`

### file list

```diff
@@ -1,275 +1,280 @@
--rw-r--r--   0        0        0     5431 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/README.md
--rw-r--r--   0        0        0      403 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/default.yaml
--rw-r--r--   0        0        0     1250 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/early_stopping.yaml
--rw-r--r--   0        0        0       80 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/layer_freeze.yaml
--rw-r--r--   0        0        0       83 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/learning_rate_monitor.yaml
--rw-r--r--   0        0        0     1298 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/model_checkpoint.yaml
--rw-r--r--   0        0        0      402 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/model_summary.yaml
--rw-r--r--   0        0        0        0 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/none.yaml
--rw-r--r--   0        0        0      160 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/outlier_detection.yaml
--rw-r--r--   0        0        0      289 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/callbacks/rich_progress_bar.yaml
--rw-r--r--   0        0        0      758 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/compile.yaml
--rw-r--r--   0        0        0     2634 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/classification/single_timepoint.yaml
--rw-r--r--   0        0        0     7077 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/gan.yaml
--rw-r--r--   0        0        0     7427 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/gan_superres.yaml
--rw-r--r--   0        0        0     6880 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/instance_seg.yaml
--rw-r--r--   0        0        0     5879 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/labelfree.yaml
--rw-r--r--   0        0        0     4374 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/mae.yaml
--rw-r--r--   0        0        0     6852 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/segmentation.yaml
--rw-r--r--   0        0        0     8222 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/segmentation_plugin.yaml
--rw-r--r--   0        0        0     7263 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/segmentation_superres.yaml
--rw-r--r--   0        0        0      450 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/lattice_nuc_sdf.yaml
--rw-r--r--   0        0        0      416 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/rot_mnist.yaml
--rw-r--r--   0        0        0      450 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/rot_mnist_vae.yaml
--rw-r--r--   0        0        0     1176 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/rotated_mnist.yaml
--rw-r--r--   0        0        0     1075 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_3d.yaml
--rw-r--r--   0        0        0      497 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_3d_npm1.yaml
--rw-r--r--   0        0        0      770 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_3d_npm_nuc_v2.yaml
--rw-r--r--   0        0        0     1802 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_3d_rotate.yaml
--rw-r--r--   0        0        0      547 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_centerslice.yaml
--rw-r--r--   0        0        0      719 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_centerslice_resize.yaml
--rw-r--r--   0        0        0      969 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_npm1.yaml
--rw-r--r--   0        0        0      312 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_spharm.yaml
--rw-r--r--   0        0        0      462 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/test/alternating_batch.yaml
--rw-r--r--   0        0        0      200 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/test/omnipose.yaml
--rw-r--r--   0        0        0      200 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/test/segmentation.yaml
--rw-r--r--   0        0        0      899 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/default.yaml
--rw-r--r--   0        0        0      125 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/fdr.yaml
--rw-r--r--   0        0        0      223 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/limit.yaml
--rw-r--r--   0        0        0      209 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/overfit.yaml
--rw-r--r--   0        0        0      182 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/profiler.yaml
--rw-r--r--   0        0        0      509 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/eval.yaml
--rw-r--r--   0        0        0      659 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/classification/per_timepoint.yaml
--rw-r--r--   0        0        0     1065 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/gan.yaml
--rw-r--r--   0        0        0     1083 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/gan_superres.yaml
--rw-r--r--   0        0        0      932 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/instance_seg.yaml
--rw-r--r--   0        0        0      854 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/labelfree.yaml
--rw-r--r--   0        0        0      892 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/mae.yaml
--rw-r--r--   0        0        0      863 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/segmentation.yaml
--rw-r--r--   0        0        0     1126 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/segmentation_plugin.yaml
--rw-r--r--   0        0        0      881 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/segmentation_superres.yaml
--rw-r--r--   0        0        0     1098 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/vit_segmentation.yaml
--rw-r--r--   0        0        0     2741 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/lattice_nuc_sdf.yaml
--rw-r--r--   0        0        0     1583 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/mnist_so2.yaml
--rw-r--r--   0        0        0      989 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_classical_3d_vae.yaml
--rw-r--r--   0        0        0     2902 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_classical_scale_inv.yaml
--rw-r--r--   0        0        0     1037 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml
--rw-r--r--   0        0        0     2825 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_scale_inv_canon_so3.yaml
--rw-r--r--   0        0        0     2568 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so2.yaml
--rw-r--r--   0        0        0     3062 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so2_scale_inv.yaml
--rw-r--r--   0        0        0     3057 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so3_scale_inv.yaml
--rw-r--r--   0        0        0     2325 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so3_vae.yaml
--rw-r--r--   0        0        0     2179 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so3_vae_seg.yaml
--rw-r--r--   0        0        0      967 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_classical_2d_vae.yaml
--rw-r--r--   0        0        0     1053 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_classical_3d_vae.yaml
--rw-r--r--   0        0        0     1385 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_so2_3d_vae.yaml
--rw-r--r--   0        0        0     1605 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_so2_3d_vae_profiling.yaml
--rw-r--r--   0        0        0     9822 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_spharm.yaml
--rw-r--r--   0        0        0     9728 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_spharm_o2.yaml
--rw-r--r--   0        0        0      309 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/extras/default.yaml
--rw-r--r--   0        0        0     1818 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/hparams_search/mnist_optuna.yaml
--rw-r--r--   0        0        0      431 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/hydra/default.yaml
--rw-r--r--   0        0        0      372 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/comet.yaml
--rw-r--r--   0        0        0      157 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/csv.yaml
--rw-r--r--   0        0        0      148 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/many_loggers.yaml
--rw-r--r--   0        0        0      166 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/mlflow.yaml
--rw-r--r--   0        0        0      277 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/neptune.yaml
--rw-r--r--   0        0        0      258 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/tensorboard.yaml
--rw-r--r--   0        0        0      522 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/wandb.yaml
--rw-r--r--   0        0        0      594 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/classification/single_timepoint.yaml
--rw-r--r--   0        0        0     1807 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/gan.yaml
--rw-r--r--   0        0        0     1948 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/gan_superres.yaml
--rw-r--r--   0        0        0     1333 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/instance_seg.yaml
--rw-r--r--   0        0        0     1237 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/labelfree.yaml
--rw-r--r--   0        0        0     1245 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/mae.yaml
--rw-r--r--   0        0        0     1333 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/segmentation.yaml
--rw-r--r--   0        0        0     1246 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/segmentation_plugin.yaml
--rw-r--r--   0        0        0     1472 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/segmentation_superres.yaml
--rw-r--r--   0        0        0     1365 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/vit_segmentation_decoder.yaml
--rw-r--r--   0        0        0      493 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/classical_image_ae.yaml
--rw-r--r--   0        0        0      536 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/classical_image_vae.yaml
--rw-r--r--   0        0        0       86 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/reconstruction_loss/spharm_gaussian.yaml
--rw-r--r--   0        0        0       76 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/reconstruction_loss/spharm_loss.yaml
--rw-r--r--   0        0        0       56 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/reconstruction_loss/spharm_mse.yaml
--rw-r--r--   0        0        0       93 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/reconstruction_loss/spharm_weighted_mse.yaml
--rw-r--r--   0        0        0      316 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/so3_canon_image_vae.yaml
--rw-r--r--   0        0        0      332 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/so3_equiv_image_vae.yaml
--rw-r--r--   0        0        0      513 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/spharm.yaml
--rw-r--r--   0        0        0      501 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/spharm_so2.yaml
--rw-r--r--   0        0        0      597 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/test/base.yaml
--rw-r--r--   0        0        0      613 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/test/simple_segmentation.yaml
--rw-r--r--   0        0        0      492 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/paths/default.yaml
--rw-r--r--   0        0        0     1745 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/train.yaml
--rw-r--r--   0        0        0       56 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/cpu.yaml
--rw-r--r--   0        0        0      394 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/ddp.yaml
--rw-r--r--   0        0        0      120 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/ddp_sim.yaml
--rw-r--r--   0        0        0      468 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/default.yaml
--rw-r--r--   0        0        0       55 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/gpu.yaml
--rw-r--r--   0        0        0       56 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/mps.yaml
--rw-r--r--   0        0        0      410 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/__init__.py
--rw-r--r--   0        0        0       31 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/api/__init__.py
--rw-r--r--   0        0        0     1040 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/api/data.py
--rw-r--r--   0        0        0     3809 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/api/model.py
--rw-r--r--   0        0        0      265 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/__init__.py
--rw-r--r--   0        0        0     6605 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/callback_utils.py
--rw-r--r--   0        0        0    11849 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/latent_walk.py
--rw-r--r--   0        0        0     1918 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/layer_freeze.py
--rw-r--r--   0        0        0     4613 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/model_utils.py
--rw-r--r--   0        0        0     6687 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/outlier_detection.py
--rw-r--r--   0        0        0     3846 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/compile.py
--rw-r--r--   0        0        0      238 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/__init__.py
--rw-r--r--   0        0        0     8481 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/readers.py
--rw-r--r--   0        0        0      251 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/__init__.py
--rw-r--r--   0        0        0     4519 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/filter.py
--rw-r--r--   0        0        0     2931 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/group_cols.py
--rw-r--r--   0        0        0     2441 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/misc.py
--rw-r--r--   0        0        0     3376 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/split.py
--rw-r--r--   0        0        0       86 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/__init__.py
--rw-r--r--   0        0        0     9014 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/czi.py
--rw-r--r--   0        0        0     1837 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/data_dict.py
--rw-r--r--   0        0        0      123 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/__init__.py
--rw-r--r--   0        0        0     7500 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/dataframe_datamodule.py
--rw-r--r--   0        0        0     4856 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py
--rw-r--r--   0        0        0    11941 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/utils.py
--rw-r--r--   0        0        0     2885 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/folder.py
--rw-r--r--   0        0        0     8044 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/smartcache.py
--rw-r--r--   0        0        0     2296 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/torchvision.py
--rw-r--r--   0        0        0     3442 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/eval.py
--rw-r--r--   0        0        0      200 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/__init__.py
--rw-r--r--   0        0        0      213 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/__init__.py
--rw-r--r--   0        0        0     2630 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/aicsimage_loader.py
--rw-r--r--   0        0        0     1908 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/monai_bio_reader.py
--rw-r--r--   0        0        0     1707 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/numpy_reader.py
--rw-r--r--   0        0        0     1885 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/ome_zarr_reader.py
--rw-r--r--   0        0        0     2464 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/polygon_loader.py
--rw-r--r--   0        0        0     1498 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/skimage_reader.py
--rw-r--r--   0        0        0      624 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/__init__.py
--rw-r--r--   0        0        0     1214 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/bright_sampler.py
--rw-r--r--   0        0        0     2468 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/clip.py
--rw-r--r--   0        0        0     2247 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/contrastadjust.py
--rw-r--r--   0        0        0     2173 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/merge.py
--rw-r--r--   0        0        0     6376 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/multiscale_cropper.py
--rw-r--r--   0        0        0     2365 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/pad.py
--rw-r--r--   0        0        0     1355 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/project.py
--rw-r--r--   0        0        0     3460 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/rotation_mask_transform.py
--rw-r--r--   0        0        0     1861 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/save.py
--rw-r--r--   0        0        0     1418 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/so2_random_rotation.py
--rw-r--r--   0        0        0     4975 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/track_transforms.py
--rw-r--r--   0        0        0       33 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/loggers/__init__.py
--rw-r--r--   0        0        0     6183 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/loggers/mlflow.py
--rw-r--r--   0        0        0        0 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/__init__.py
--rw-r--r--   0        0        0     7267 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/base_model.py
--rw-r--r--   0        0        0     3298 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/basic_model.py
--rw-r--r--   0        0        0      105 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/classification/__init__.py
--rw-r--r--   0        0        0     4454 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/classification/classification.py
--rw-r--r--   0        0        0     3047 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/classification/timepoint_classification.py
--rw-r--r--   0        0        0       38 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/handlers/__init__.py
--rw-r--r--   0        0        0     2832 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/handlers/base_handler.py
--rw-r--r--   0        0        0     1133 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/handlers/image_handler.py
--rw-r--r--   0        0        0     1139 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/handlers/load_image_patch.py
--rw-r--r--   0        0        0       60 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/im2im/__init__.py
--rw-r--r--   0        0        0     6319 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/gan.py
--rw-r--r--   0        0        0     8946 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/multi_task.py
--rw-r--r--   0        0        0      324 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/__init__.py
--rw-r--r--   0        0        0    21568 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/instance_seg.py
--rw-r--r--   0        0        0     1531 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/noise_annealer.py
--rw-r--r--   0        0        0      125 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/__init__.py
--rw-r--r--   0        0        0     2410 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py
--rw-r--r--   0        0        0      835 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py
--rw-r--r--   0        0        0     1287 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py
--rw-r--r--   0        0        0       32 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/utils/__init__.py
--rw-r--r--   0        0        0     1264 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/utils/mlflow.py
--rw-r--r--   0        0        0      268 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/utils/utils.py
--rw-r--r--   0        0        0      284 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/__init__.py
--rw-r--r--   0        0        0    10624 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/base_vae.py
--rw-r--r--   0        0        0    10648 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/image_canon_vae.py
--rw-r--r--   0        0        0    11242 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/image_encoder.py
--rw-r--r--   0        0        0     8223 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/image_vae.py
--rw-r--r--   0        0        0     9890 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/latent_loss_vae.py
--rw-r--r--   0        0        0       39 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/__init__.py
--rw-r--r--   0        0        0     3653 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py
--rw-r--r--   0        0        0     4323 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py
--rw-r--r--   0        0        0    11244 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/point_cloud_vae.py
--rw-r--r--   0        0        0      144 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/__init__.py
--rw-r--r--   0        0        0      574 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/abstract_prior.py
--rw-r--r--   0        0        0     5530 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/gaussian.py
--rw-r--r--   0        0        0      408 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/identity_prior.py
--rw-r--r--   0        0        0     1609 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/joint_prior.py
--rw-r--r--   0        0        0     1280 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/tabular_vae.py
--rw-r--r--   0        0        0      305 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/__init__.py
--rw-r--r--   0        0        0      118 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/discriminators/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/discriminators/multi_scale_discriminator.py
--rw-r--r--   0        0        0     3816 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/discriminators/n_layer_discriminator.py
--rw-r--r--   0        0        0      151 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/__init__.py
--rw-r--r--   0        0        0     3802 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/base_head.py
--rw-r--r--   0        0        0     3115 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/gan_head.py
--rw-r--r--   0        0        0     2850 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/gan_head_superres.py
--rw-r--r--   0        0        0      928 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/mae_head.py
--rw-r--r--   0        0        0     2033 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/mask_head.py
--rw-r--r--   0        0        0     4415 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/res_blocks_head.py
--rw-r--r--   0        0        0     1042 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/hr_skip.py
--rw-r--r--   0        0        0      592 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/__init__.py
--rw-r--r--   0        0        0     1071 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/adversarial_loss.py
--rw-r--r--   0        0        0     1119 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/chamfer_loss.py
--rw-r--r--   0        0        0     1046 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/continuous_bernoulli.py
--rw-r--r--   0        0        0      671 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/cosine_loss.py
--rw-r--r--   0        0        0     4431 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/gan_loss.py
--rw-r--r--   0        0        0      917 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/gaussian_nll_loss.py
--rw-r--r--   0        0        0      873 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/geomloss.py
--rw-r--r--   0        0        0     2155 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/loss_wrapper.py
--rw-r--r--   0        0        0     1015 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/spharm_loss.py
--rw-r--r--   0        0        0      895 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/threshold_loss.py
--rw-r--r--   0        0        0     1105 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/weibull.py
--rw-r--r--   0        0        0      675 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/weighted_mse_loss.py
--rw-r--r--   0        0        0      958 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/mlp.py
--rw-r--r--   0        0        0       61 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/__init__.py
--rw-r--r--   0        0        0    13372 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/dgcnn.py
--rw-r--r--   0        0        0     2732 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/folding_net.py
--rw-r--r--   0        0        0     4934 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/graph_functions.py
--rw-r--r--   0        0        0     5754 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/vnn.py
--rw-r--r--   0        0        0     6848 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/res_unit.py
--rw-r--r--   0        0        0     2555 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/spatial_transformer.py
--rw-r--r--   0        0        0     2571 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/track_sequence_predictor.py
--rw-r--r--   0        0        0      165 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/__init__.py
--rw-r--r--   0        0        0      171 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/__init__.py
--rw-r--r--   0        0        0     4427 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/cross_attention.py
--rw-r--r--   0        0        0      848 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/intermediate_weigher.py
--rw-r--r--   0        0        0     5249 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/patchify.py
--rw-r--r--   0        0        0     5577 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/cross_mae.py
--rw-r--r--   0        0        0    10645 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/mae.py
--rw-r--r--   0        0        0    10199 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/seg.py
--rw-r--r--   0        0        0      208 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/utils.py
--rw-r--r--   0        0        0        0 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/point_cloud/__init__.py
--rw-r--r--   0        0        0       40 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/point_cloud/io/__init__.py
--rw-r--r--   0        0        0     4992 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/point_cloud/io/read_pcloud.py
--rw-r--r--   0        0        0     5355 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/train.py
--rw-r--r--   0        0        0      333 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/utils/__init__.py
--rw-r--r--   0        0        0     1791 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/utils/config.py
--rw-r--r--   0        0        0     2391 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/download_test_data.py
--rw-r--r--   0        0        0     2359 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/dummy_dataset.py
--rw-r--r--   0        0        0      671 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/pylogger.py
--rw-r--r--   0        0        0     3326 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/rich_utils.py
--rw-r--r--   0        0        0     3808 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/rotation.py
--rw-r--r--   0        0        0      237 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/spharm/__init__.py
--rw-r--r--   0        0        0     6015 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/spharm/reconstruction.py
--rw-r--r--   0        0        0     4360 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/spharm/rotation.py
--rw-r--r--   0        0        0     7103 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/template_utils.py
--rw-r--r--   0        0        0     2887 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      929 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/api/test_model.py
--rw-r--r--   0        0        0     3599 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/helpers/__init__.py
--rw-r--r--   0        0        0      857 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/helpers/package_available.py
--rw-r--r--   0        0        0     4307 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/helpers/run_if.py
--rw-r--r--   0        0        0   259123 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/resources/rand_im.tif
--rw-r--r--   0        0        0      336 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/resources/test.csv
--rw-r--r--   0        0        0      635 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/resources/train.csv
--rw-r--r--   0        0        0      336 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/resources/valid.csv
--rw-r--r--   0        0        0     2675 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_alternating_batch_sampler.py
--rw-r--r--   0        0        0     1434 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_configs.py
--rw-r--r--   0        0        0     1604 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_eval.py
--rw-r--r--   0        0        0     3730 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_mlflow_logger.py
--rw-r--r--   0        0        0     1119 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_polygon_loader.py
--rw-r--r--   0        0        0     2243 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_train.py
--rw-r--r--   0        0        0      143 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/utils.py
--rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 cyto-dl-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     5431 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/README.md
+-rw-r--r--   0        0        0      403 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/default.yaml
+-rw-r--r--   0        0        0     1250 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/early_stopping.yaml
+-rw-r--r--   0        0        0       80 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/layer_freeze.yaml
+-rw-r--r--   0        0        0       83 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/learning_rate_monitor.yaml
+-rw-r--r--   0        0        0     1298 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/model_checkpoint.yaml
+-rw-r--r--   0        0        0      402 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/model_summary.yaml
+-rw-r--r--   0        0        0        0 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/none.yaml
+-rw-r--r--   0        0        0      160 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/outlier_detection.yaml
+-rw-r--r--   0        0        0      289 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/rich_progress_bar.yaml
+-rw-r--r--   0        0        0      758 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/compile.yaml
+-rw-r--r--   0        0        0     2634 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/classification/single_timepoint.yaml
+-rw-r--r--   0        0        0     7077 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/gan.yaml
+-rw-r--r--   0        0        0     7427 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/gan_superres.yaml
+-rw-r--r--   0        0        0     6880 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/instance_seg.yaml
+-rw-r--r--   0        0        0     5879 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/labelfree.yaml
+-rw-r--r--   0        0        0     4374 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/mae.yaml
+-rw-r--r--   0        0        0     6852 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/segmentation.yaml
+-rw-r--r--   0        0        0     8053 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/segmentation_plugin.yaml
+-rw-r--r--   0        0        0     7263 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/segmentation_superres.yaml
+-rw-r--r--   0        0        0      450 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/lattice_nuc_sdf.yaml
+-rw-r--r--   0        0        0      416 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/rot_mnist.yaml
+-rw-r--r--   0        0        0      450 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/rot_mnist_vae.yaml
+-rw-r--r--   0        0        0     1176 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/rotated_mnist.yaml
+-rw-r--r--   0        0        0     1075 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_3d.yaml
+-rw-r--r--   0        0        0      497 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_3d_npm1.yaml
+-rw-r--r--   0        0        0      770 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_3d_npm_nuc_v2.yaml
+-rw-r--r--   0        0        0     1802 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_3d_rotate.yaml
+-rw-r--r--   0        0        0      547 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_centerslice.yaml
+-rw-r--r--   0        0        0      719 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_centerslice_resize.yaml
+-rw-r--r--   0        0        0      969 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_npm1.yaml
+-rw-r--r--   0        0        0      312 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_spharm.yaml
+-rw-r--r--   0        0        0      462 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/data/test/alternating_batch.yaml
+-rw-r--r--   0        0        0      200 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/data/test/omnipose.yaml
+-rw-r--r--   0        0        0      200 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/data/test/segmentation.yaml
+-rw-r--r--   0        0        0      899 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/default.yaml
+-rw-r--r--   0        0        0      125 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/fdr.yaml
+-rw-r--r--   0        0        0      223 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/limit.yaml
+-rw-r--r--   0        0        0      209 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/overfit.yaml
+-rw-r--r--   0        0        0      182 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/profiler.yaml
+-rw-r--r--   0        0        0      509 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/eval.yaml
+-rw-r--r--   0        0        0      659 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/classification/per_timepoint.yaml
+-rw-r--r--   0        0        0     1065 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/gan.yaml
+-rw-r--r--   0        0        0     1083 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/gan_superres.yaml
+-rw-r--r--   0        0        0      932 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/instance_seg.yaml
+-rw-r--r--   0        0        0      854 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/labelfree.yaml
+-rw-r--r--   0        0        0      892 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/mae.yaml
+-rw-r--r--   0        0        0      863 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/segmentation.yaml
+-rw-r--r--   0        0        0     1622 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/segmentation_plugin.yaml
+-rw-r--r--   0        0        0      881 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/segmentation_superres.yaml
+-rw-r--r--   0        0        0     1098 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/vit_segmentation.yaml
+-rw-r--r--   0        0        0     2741 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/lattice_nuc_sdf.yaml
+-rw-r--r--   0        0        0     1583 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/mnist_so2.yaml
+-rw-r--r--   0        0        0      989 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_classical_3d_vae.yaml
+-rw-r--r--   0        0        0     2902 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_classical_scale_inv.yaml
+-rw-r--r--   0        0        0     1037 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml
+-rw-r--r--   0        0        0     2825 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_scale_inv_canon_so3.yaml
+-rw-r--r--   0        0        0     2568 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so2.yaml
+-rw-r--r--   0        0        0     3062 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so2_scale_inv.yaml
+-rw-r--r--   0        0        0     3057 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so3_scale_inv.yaml
+-rw-r--r--   0        0        0     2325 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so3_vae.yaml
+-rw-r--r--   0        0        0     2179 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so3_vae_seg.yaml
+-rw-r--r--   0        0        0      967 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_classical_2d_vae.yaml
+-rw-r--r--   0        0        0     1053 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_classical_3d_vae.yaml
+-rw-r--r--   0        0        0     1385 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_so2_3d_vae.yaml
+-rw-r--r--   0        0        0     1605 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_so2_3d_vae_profiling.yaml
+-rw-r--r--   0        0        0     9822 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_spharm.yaml
+-rw-r--r--   0        0        0     9728 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_spharm_o2.yaml
+-rw-r--r--   0        0        0      309 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/extras/default.yaml
+-rw-r--r--   0        0        0     1818 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/hparams_search/mnist_optuna.yaml
+-rw-r--r--   0        0        0      431 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/hydra/default.yaml
+-rw-r--r--   0        0        0      372 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/comet.yaml
+-rw-r--r--   0        0        0      157 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/csv.yaml
+-rw-r--r--   0        0        0      148 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/many_loggers.yaml
+-rw-r--r--   0        0        0      166 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/mlflow.yaml
+-rw-r--r--   0        0        0      277 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/neptune.yaml
+-rw-r--r--   0        0        0      258 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/tensorboard.yaml
+-rw-r--r--   0        0        0      522 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/wandb.yaml
+-rw-r--r--   0        0        0      594 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/classification/single_timepoint.yaml
+-rw-r--r--   0        0        0     1807 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/gan.yaml
+-rw-r--r--   0        0        0     1948 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/gan_superres.yaml
+-rw-r--r--   0        0        0     1333 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/instance_seg.yaml
+-rw-r--r--   0        0        0     1237 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/labelfree.yaml
+-rw-r--r--   0        0        0     1245 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/mae.yaml
+-rw-r--r--   0        0        0     1333 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/segmentation.yaml
+-rw-r--r--   0        0        0     1252 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/segmentation_plugin.yaml
+-rw-r--r--   0        0        0     1472 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/segmentation_superres.yaml
+-rw-r--r--   0        0        0     1365 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/vit_segmentation_decoder.yaml
+-rw-r--r--   0        0        0      493 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/classical_image_ae.yaml
+-rw-r--r--   0        0        0      536 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/classical_image_vae.yaml
+-rw-r--r--   0        0        0       86 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/reconstruction_loss/spharm_gaussian.yaml
+-rw-r--r--   0        0        0       76 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/reconstruction_loss/spharm_loss.yaml
+-rw-r--r--   0        0        0       56 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/reconstruction_loss/spharm_mse.yaml
+-rw-r--r--   0        0        0       93 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/reconstruction_loss/spharm_weighted_mse.yaml
+-rw-r--r--   0        0        0      316 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/so3_canon_image_vae.yaml
+-rw-r--r--   0        0        0      332 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/so3_equiv_image_vae.yaml
+-rw-r--r--   0        0        0      513 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/spharm.yaml
+-rw-r--r--   0        0        0      501 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/spharm_so2.yaml
+-rw-r--r--   0        0        0      597 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/test/base.yaml
+-rw-r--r--   0        0        0      613 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/test/simple_segmentation.yaml
+-rw-r--r--   0        0        0      492 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/paths/default.yaml
+-rw-r--r--   0        0        0     1745 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/train.yaml
+-rw-r--r--   0        0        0       56 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/cpu.yaml
+-rw-r--r--   0        0        0      394 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/ddp.yaml
+-rw-r--r--   0        0        0      120 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/ddp_sim.yaml
+-rw-r--r--   0        0        0      468 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/default.yaml
+-rw-r--r--   0        0        0       55 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/gpu.yaml
+-rw-r--r--   0        0        0       56 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/mps.yaml
+-rw-r--r--   0        0        0      410 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/__init__.py
+-rw-r--r--   0        0        0      111 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/cyto_dl_model/__init__.py
+-rw-r--r--   0        0        0     5137 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/cyto_dl_model/cyto_dl_base_model.py
+-rw-r--r--   0        0        0     3766 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/cyto_dl_model/segmentation_plugin_model.py
+-rw-r--r--   0        0        0     1040 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/data.py
+-rw-r--r--   0        0        0     4007 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/model.py
+-rw-r--r--   0        0        0      265 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/__init__.py
+-rw-r--r--   0        0        0     6605 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/callback_utils.py
+-rw-r--r--   0        0        0    11849 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/latent_walk.py
+-rw-r--r--   0        0        0     1918 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/layer_freeze.py
+-rw-r--r--   0        0        0     4613 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/model_utils.py
+-rw-r--r--   0        0        0     6687 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/outlier_detection.py
+-rw-r--r--   0        0        0     3846 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/compile.py
+-rw-r--r--   0        0        0      238 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/__init__.py
+-rw-r--r--   0        0        0     8481 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/readers.py
+-rw-r--r--   0        0        0      251 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/__init__.py
+-rw-r--r--   0        0        0     4519 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/filter.py
+-rw-r--r--   0        0        0     2931 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/group_cols.py
+-rw-r--r--   0        0        0     2441 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/misc.py
+-rw-r--r--   0        0        0     3376 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/split.py
+-rw-r--r--   0        0        0       86 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/__init__.py
+-rw-r--r--   0        0        0     8995 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/czi.py
+-rw-r--r--   0        0        0     1837 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/data_dict.py
+-rw-r--r--   0        0        0      123 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/__init__.py
+-rw-r--r--   0        0        0     7500 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/dataframe_datamodule.py
+-rw-r--r--   0        0        0     4856 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py
+-rw-r--r--   0        0        0    11941 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/utils.py
+-rw-r--r--   0        0        0     2885 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/folder.py
+-rw-r--r--   0        0        0     8030 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/smartcache.py
+-rw-r--r--   0        0        0     2296 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/torchvision.py
+-rw-r--r--   0        0        0     3442 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/eval.py
+-rw-r--r--   0        0        0      200 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/__init__.py
+-rw-r--r--   0        0        0      213 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/__init__.py
+-rw-r--r--   0        0        0     2621 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/aicsimage_loader.py
+-rw-r--r--   0        0        0     1892 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/monai_bio_reader.py
+-rw-r--r--   0        0        0     1707 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/numpy_reader.py
+-rw-r--r--   0        0        0     1885 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/ome_zarr_reader.py
+-rw-r--r--   0        0        0     2550 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/polygon_loader.py
+-rw-r--r--   0        0        0     1498 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/skimage_reader.py
+-rw-r--r--   0        0        0      624 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/__init__.py
+-rw-r--r--   0        0        0     1214 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/bright_sampler.py
+-rw-r--r--   0        0        0     2468 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/clip.py
+-rw-r--r--   0        0        0     2247 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/contrastadjust.py
+-rw-r--r--   0        0        0     2586 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/merge.py
+-rw-r--r--   0        0        0     6376 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/multiscale_cropper.py
+-rw-r--r--   0        0        0     2365 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/pad.py
+-rw-r--r--   0        0        0     1355 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/project.py
+-rw-r--r--   0        0        0     3460 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/rotation_mask_transform.py
+-rw-r--r--   0        0        0     1855 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/save.py
+-rw-r--r--   0        0        0     1418 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/so2_random_rotation.py
+-rw-r--r--   0        0        0     4975 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/track_transforms.py
+-rw-r--r--   0        0        0       33 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/loggers/__init__.py
+-rw-r--r--   0        0        0     6183 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/loggers/mlflow.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/__init__.py
+-rw-r--r--   0        0        0     7267 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/base_model.py
+-rw-r--r--   0        0        0     3298 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/basic_model.py
+-rw-r--r--   0        0        0      105 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/classification/__init__.py
+-rw-r--r--   0        0        0     4448 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/classification/classification.py
+-rw-r--r--   0        0        0     3047 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/classification/timepoint_classification.py
+-rw-r--r--   0        0        0       38 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/handlers/__init__.py
+-rw-r--r--   0        0        0     2832 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/handlers/base_handler.py
+-rw-r--r--   0        0        0     1133 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/handlers/image_handler.py
+-rw-r--r--   0        0        0     1139 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/handlers/load_image_patch.py
+-rw-r--r--   0        0        0       60 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/__init__.py
+-rw-r--r--   0        0        0     6319 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/gan.py
+-rw-r--r--   0        0        0     8946 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/multi_task.py
+-rw-r--r--   0        0        0      324 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/__init__.py
+-rw-r--r--   0        0        0    21568 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/instance_seg.py
+-rw-r--r--   0        0        0     1531 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/noise_annealer.py
+-rw-r--r--   0        0        0      125 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/__init__.py
+-rw-r--r--   0        0        0     2410 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py
+-rw-r--r--   0        0        0      927 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py
+-rw-r--r--   0        0        0     1287 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py
+-rw-r--r--   0        0        0       32 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/utils/__init__.py
+-rw-r--r--   0        0        0     1264 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/utils/mlflow.py
+-rw-r--r--   0        0        0      268 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/utils/utils.py
+-rw-r--r--   0        0        0      284 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/__init__.py
+-rw-r--r--   0        0        0    10624 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/base_vae.py
+-rw-r--r--   0        0        0    10648 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/image_canon_vae.py
+-rw-r--r--   0        0        0    11242 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/image_encoder.py
+-rw-r--r--   0        0        0     8223 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/image_vae.py
+-rw-r--r--   0        0        0     9890 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/latent_loss_vae.py
+-rw-r--r--   0        0        0       39 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/__init__.py
+-rw-r--r--   0        0        0     3653 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py
+-rw-r--r--   0        0        0     4323 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py
+-rw-r--r--   0        0        0    11244 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/point_cloud_vae.py
+-rw-r--r--   0        0        0      144 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/abstract_prior.py
+-rw-r--r--   0        0        0     5530 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/gaussian.py
+-rw-r--r--   0        0        0      408 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/identity_prior.py
+-rw-r--r--   0        0        0     1609 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/joint_prior.py
+-rw-r--r--   0        0        0     1280 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/tabular_vae.py
+-rw-r--r--   0        0        0      305 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/__init__.py
+-rw-r--r--   0        0        0      118 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/discriminators/__init__.py
+-rw-r--r--   0        0        0     1695 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/discriminators/multi_scale_discriminator.py
+-rw-r--r--   0        0        0     3816 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/discriminators/n_layer_discriminator.py
+-rw-r--r--   0        0        0      183 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/__init__.py
+-rw-r--r--   0        0        0     3796 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/base_head.py
+-rw-r--r--   0        0        0     3115 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/gan_head.py
+-rw-r--r--   0        0        0     2850 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/gan_head_superres.py
+-rw-r--r--   0        0        0      928 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/mae_head.py
+-rw-r--r--   0        0        0     1984 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/mask_head.py
+-rw-r--r--   0        0        0     4415 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/res_blocks_head.py
+-rw-r--r--   0        0        0     1042 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/hr_skip.py
+-rw-r--r--   0        0        0      592 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/__init__.py
+-rw-r--r--   0        0        0     1071 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/adversarial_loss.py
+-rw-r--r--   0        0        0     1119 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/chamfer_loss.py
+-rw-r--r--   0        0        0     1046 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/continuous_bernoulli.py
+-rw-r--r--   0        0        0      671 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/cosine_loss.py
+-rw-r--r--   0        0        0     4431 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/gan_loss.py
+-rw-r--r--   0        0        0      917 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/gaussian_nll_loss.py
+-rw-r--r--   0        0        0      873 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/geomloss.py
+-rw-r--r--   0        0        0     2155 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/loss_wrapper.py
+-rw-r--r--   0        0        0     1015 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/spharm_loss.py
+-rw-r--r--   0        0        0      895 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/threshold_loss.py
+-rw-r--r--   0        0        0     1105 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/weibull.py
+-rw-r--r--   0        0        0      675 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/weighted_mse_loss.py
+-rw-r--r--   0        0        0      958 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/mlp.py
+-rw-r--r--   0        0        0       61 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/__init__.py
+-rw-r--r--   0        0        0    13372 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/dgcnn.py
+-rw-r--r--   0        0        0     2732 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/folding_net.py
+-rw-r--r--   0        0        0     4934 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/graph_functions.py
+-rw-r--r--   0        0        0     5754 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/vnn.py
+-rw-r--r--   0        0        0     6848 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/res_unit.py
+-rw-r--r--   0        0        0     2555 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/spatial_transformer.py
+-rw-r--r--   0        0        0     2571 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/track_sequence_predictor.py
+-rw-r--r--   0        0        0      165 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/__init__.py
+-rw-r--r--   0        0        0     4427 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/cross_attention.py
+-rw-r--r--   0        0        0      848 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/intermediate_weigher.py
+-rw-r--r--   0        0        0     5249 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/patchify.py
+-rw-r--r--   0        0        0     5577 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/cross_mae.py
+-rw-r--r--   0        0        0    10645 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/mae.py
+-rw-r--r--   0        0        0    10199 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/seg.py
+-rw-r--r--   0        0        0      208 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/utils.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/point_cloud/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/point_cloud/io/__init__.py
+-rw-r--r--   0        0        0     4992 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/point_cloud/io/read_pcloud.py
+-rw-r--r--   0        0        0     5355 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/train.py
+-rw-r--r--   0        0        0      333 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/__init__.py
+-rw-r--r--   0        0        0     1791 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/config.py
+-rw-r--r--   0        0        0     2391 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/download_test_data.py
+-rw-r--r--   0        0        0     2359 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/dummy_dataset.py
+-rw-r--r--   0        0        0      671 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/pylogger.py
+-rw-r--r--   0        0        0     3326 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/rich_utils.py
+-rw-r--r--   0        0        0     3808 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/rotation.py
+-rw-r--r--   0        0        0      237 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/spharm/__init__.py
+-rw-r--r--   0        0        0     6015 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/spharm/reconstruction.py
+-rw-r--r--   0        0        0     4360 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/spharm/rotation.py
+-rw-r--r--   0        0        0     7103 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/template_utils.py
+-rw-r--r--   0        0        0     2849 2024-05-03 16:17:29.124416 cyto-dl-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0       36 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/api/cyto_dl_model/bad_config.yaml
+-rw-r--r--   0        0        0     5602 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/api/cyto_dl_model/test_segmentation_plugin_model.py
+-rw-r--r--   0        0        0      929 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/api/test_model.py
+-rw-r--r--   0        0        0     3599 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/helpers/package_available.py
+-rw-r--r--   0        0        0     4307 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/helpers/run_if.py
+-rw-r--r--   0        0        0   259123 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/resources/rand_im.tif
+-rw-r--r--   0        0        0      336 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/resources/test.csv
+-rw-r--r--   0        0        0      635 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/resources/train.csv
+-rw-r--r--   0        0        0      336 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/resources/valid.csv
+-rw-r--r--   0        0        0     2675 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_alternating_batch_sampler.py
+-rw-r--r--   0        0        0     1434 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_configs.py
+-rw-r--r--   0        0        0     1604 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_eval.py
+-rw-r--r--   0        0        0     3730 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_mlflow_logger.py
+-rw-r--r--   0        0        0     1119 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_polygon_loader.py
+-rw-r--r--   0        0        0     2243 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_train.py
+-rw-r--r--   0        0        0      143 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/utils.py
+-rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 cyto-dl-0.1.6/PKG-INFO
```

### Comparing `cyto-dl-0.1.5/README.md` & `cyto-dl-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/callbacks/early_stopping.yaml` & `cyto-dl-0.1.6/configs/callbacks/early_stopping.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/callbacks/model_checkpoint.yaml` & `cyto-dl-0.1.6/configs/callbacks/model_checkpoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/compile.yaml` & `cyto-dl-0.1.6/configs/compile.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/classification/single_timepoint.yaml` & `cyto-dl-0.1.6/configs/data/classification/single_timepoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/im2im/gan.yaml` & `cyto-dl-0.1.6/configs/data/im2im/gan.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/im2im/gan_superres.yaml` & `cyto-dl-0.1.6/configs/data/im2im/gan_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/im2im/instance_seg.yaml` & `cyto-dl-0.1.6/configs/data/im2im/instance_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/im2im/labelfree.yaml` & `cyto-dl-0.1.6/configs/data/im2im/labelfree.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/im2im/mae.yaml` & `cyto-dl-0.1.6/configs/data/im2im/mae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/im2im/segmentation.yaml` & `cyto-dl-0.1.6/configs/data/im2im/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/im2im/segmentation_plugin.yaml` & `cyto-dl-0.1.6/configs/data/im2im/segmentation_plugin.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 _target_: cyto_dl.datamodules.dataframe.DataframeDatamodule
 
 path:
 cache_dir:
 
-num_workers: 0
+num_workers: 4
 batch_size: 1
 pin_memory: True
 split_column:
 columns:
   - ${source_col}
   - ${target_col1}
   - ${target_col2}
@@ -15,14 +15,16 @@
   - ${exclude_mask_col}
   - ${base_image_col}
 
 transforms:
   train:
     _target_: monai.transforms.Compose
     transforms:
+      # remove nan keys
+      - _target_: cyto_dl.datamodules.dataframe.utils.RemoveNaNKeysd
       # load
       - _target_: monai.transforms.LoadImaged
         keys: ${source_col}
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: ${input_channel}
@@ -30,18 +32,27 @@
         keys: ${target_col1}
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: 0
       - _target_: monai.transforms.LoadImaged
         keys: ${target_col2}
+        allow_missing_keys: True
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: 0
+      - _target_: monai.transforms.ThresholdIntensityd
+        allow_missing_keys: True
+        keys:
+          - ${target_col1}
+          - ${target_col2}
+        threshold: 0.1
+        above: False
+        cval: 1
       # load merging mask - assumed not to exist by default
       - _target_: cyto_dl.image.io.PolygonLoaderd
         keys:
           - ${merge_mask_col}
         shape_reference_key: ${target_col1}
         missing_key_mode: "ignore"
       # load excluding mask - assumed to be all ones by default
@@ -58,76 +69,37 @@
       - _target_: cyto_dl.image.transforms.merge.Merged
         mask_key: ${merge_mask_col}
         image_keys:
           - ${target_col1}
           - ${target_col2}
         base_image_key: ${base_image_col}
         output_name: target
-      #crop
-      - _target_: cyto_dl.image.transforms.RandomMultiScaleCropd
-        keys:
-          - ${source_col}
-          - target
-          - ${exclude_mask_col}
-        patch_shape: ${data._aux.patch_shape}
-        patch_per_image: 1
-        scales_dict: ${kv_to_dict:${data._aux._scales_dict}}
 
-      # augmentation
-      - _target_: monai.transforms.RandRotate90d
-        keys:
-          - ${source_col}
-          - target
-          - ${exclude_mask_col}
-        prob: 0.5
-        spatial_axes: [0, 1]
-      - _target_: monai.transforms.RandFlipd
-        keys:
-          - ${source_col}
-          - target
-          - ${exclude_mask_col}
-        prob: 0.5
-        spatial_axis: 0
-      - _target_: monai.transforms.RandFlipd
-        keys:
-          - ${source_col}
-          - target
-          - ${exclude_mask_col}
-        prob: 0.5
-        spatial_axis: 1
-      - _target_: monai.transforms.RandHistogramShiftd
-        prob: 0.1
-        keys:
-          - ${source_col}
-          - target
-          - ${exclude_mask_col}
-        num_control_points: [90, 500]
-      - _target_: monai.transforms.RandStdShiftIntensityd
-        prob: 0.1
-        keys:
-          - ${source_col}
-          - target
-          - ${exclude_mask_col}
-        factors: 0.1
-      - _target_: monai.transforms.RandAdjustContrastd
-        prob: 0.1
+      - _target_: monai.transforms.ToTensord
         keys:
           - ${source_col}
           - target
           - ${exclude_mask_col}
-        gamma: [0.9, 1.5]
-      - _target_: monai.transforms.ToTensord
+        dtype: float16
+
+      #crop
+      - _target_: cyto_dl.image.transforms.RandomMultiScaleCropd
         keys:
           - ${source_col}
           - target
           - ${exclude_mask_col}
+        patch_shape: ${data._aux.patch_shape}
+        patch_per_image: ${data._aux.patch_per_image}
+        scales_dict: ${kv_to_dict:${data._aux._scales_dict}}
 
   test:
     _target_: monai.transforms.Compose
     transforms:
+      # remove nan keys
+      - _target_: cyto_dl.datamodules.dataframe.utils.RemoveNaNKeysd
       # load
       - _target_: monai.transforms.LoadImaged
         keys: ${source_col}
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: ${input_channel}
@@ -135,14 +107,15 @@
         keys: ${target_col1}
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: 0
       - _target_: monai.transforms.LoadImaged
         keys: ${target_col2}
+        allow_missing_keys: True
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: 0
       # load merging mask - assumed not to exist by default
       - _target_: cyto_dl.image.io.PolygonLoaderd
         keys:
@@ -154,53 +127,55 @@
         keys:
           - ${exclude_mask_col}
         shape_reference_key: ${target_col1}
         missing_key_mode: "create"
       # normalize
       - _target_: monai.transforms.NormalizeIntensityd
         keys: ${source_col}
-
         channel_wise: True
       # merge masks
       - _target_: cyto_dl.image.transforms.merge.Merged
         mask_key: ${merge_mask_col}
         image_keys:
           - ${target_col1}
           - ${target_col2}
         base_image_key: ${base_image_col}
         output_name: target
+
       - _target_: monai.transforms.ToTensord
         keys:
           - ${source_col}
           - target
           - ${exclude_mask_col}
+        dtype: float16
 
   predict:
     _target_: monai.transforms.Compose
     transforms:
+      - _target_: cyto_dl.datamodules.dataframe.utils.RemoveNaNKeysd
       # load
       - _target_: monai.transforms.LoadImaged
         keys: ${source_col}
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: ${input_channel}
       # normalize
       - _target_: monai.transforms.NormalizeIntensityd
         keys: ${source_col}
         channel_wise: True
       - _target_: monai.transforms.ToTensord
         keys:
           - ${source_col}
-          - target
-          - ${exclude_mask_col}
 
   valid:
     _target_: monai.transforms.Compose
     transforms:
+      # remove nan keys
+      - _target_: cyto_dl.datamodules.dataframe.utils.RemoveNaNKeysd
       # load
       - _target_: monai.transforms.LoadImaged
         keys: ${source_col}
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: ${input_channel}
@@ -208,19 +183,28 @@
         keys: ${target_col1}
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: 0
       - _target_: monai.transforms.LoadImaged
         keys: ${target_col2}
+        allow_missing_keys: True
         reader:
           - _target_: cyto_dl.image.io.MonaiBioReader
             dimension_order_out: ${eval:'"CZYX" if ${spatial_dims}==3 else "CYX"'}
             C: 0
 
+      - _target_: monai.transforms.ThresholdIntensityd
+        allow_missing_keys: True
+        keys:
+          - ${target_col1}
+          - ${target_col2}
+        threshold: 0.1
+        above: False
+        cval: 1
       # load merging mask - assumed not to exist by default
       - _target_: cyto_dl.image.io.PolygonLoaderd
         keys:
           - ${merge_mask_col}
         shape_reference_key: ${target_col1}
         missing_key_mode: "ignore"
       # load excluding mask - assumed to be all ones by default
@@ -240,29 +224,33 @@
         mask_key: ${merge_mask_col}
         image_keys:
           - ${target_col1}
           - ${target_col2}
         base_image_key: ${base_image_col}
         output_name: target
 
-      # #crop
-      - _target_: cyto_dl.image.transforms.RandomMultiScaleCropd
+      - _target_: monai.transforms.ToTensord
         keys:
           - ${source_col}
           - target
           - ${exclude_mask_col}
-        patch_shape: ${data._aux.patch_shape}
-        patch_per_image: 1
-        scales_dict: ${kv_to_dict:${data._aux._scales_dict}}
-      - _target_: monai.transforms.ToTensord
+        dtype: float16
+
+      # #crop
+      - _target_: cyto_dl.image.transforms.RandomMultiScaleCropd
         keys:
           - ${source_col}
           - target
           - ${exclude_mask_col}
+        patch_shape: ${data._aux.patch_shape}
+        patch_per_image: ${data._aux.patch_per_image}
+        scales_dict: ${kv_to_dict:${data._aux._scales_dict}}
+
 _aux:
+  patch_per_image: 1
   _scales_dict:
     - - target
       - [1]
     - - ${source_col}
       - [1]
     - - ${exclude_mask_col}
       - [1]
```

### Comparing `cyto-dl-0.1.5/configs/data/im2im/segmentation_superres.yaml` & `cyto-dl-0.1.6/configs/data/im2im/segmentation_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/private/rotated_mnist.yaml` & `cyto-dl-0.1.6/configs/data/private/rotated_mnist.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/private/variance_3d.yaml` & `cyto-dl-0.1.6/configs/data/private/variance_3d.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/private/variance_3d_npm_nuc_v2.yaml` & `cyto-dl-0.1.6/configs/data/private/variance_3d_npm_nuc_v2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/private/variance_3d_rotate.yaml` & `cyto-dl-0.1.6/configs/data/private/variance_3d_rotate.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/private/variance_centerslice.yaml` & `cyto-dl-0.1.6/configs/data/private/variance_centerslice.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/private/variance_centerslice_resize.yaml` & `cyto-dl-0.1.6/configs/data/private/variance_centerslice_resize.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/data/private/variance_npm1.yaml` & `cyto-dl-0.1.6/configs/data/private/variance_npm1.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/debug/default.yaml` & `cyto-dl-0.1.6/configs/debug/default.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/classification/per_timepoint.yaml` & `cyto-dl-0.1.6/configs/experiment/classification/per_timepoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/im2im/gan.yaml` & `cyto-dl-0.1.6/configs/experiment/im2im/gan.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/im2im/gan_superres.yaml` & `cyto-dl-0.1.6/configs/experiment/im2im/gan_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/im2im/instance_seg.yaml` & `cyto-dl-0.1.6/configs/experiment/im2im/instance_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/im2im/labelfree.yaml` & `cyto-dl-0.1.6/configs/experiment/im2im/labelfree.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/im2im/mae.yaml` & `cyto-dl-0.1.6/configs/experiment/im2im/mae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/im2im/segmentation.yaml` & `cyto-dl-0.1.6/configs/experiment/im2im/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/im2im/segmentation_plugin.yaml` & `cyto-dl-0.1.6/configs/experiment/im2im/vit_segmentation.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 # @package _global_
+
 # to execute this experiment run:
 # python train.py experiment=example
+
 defaults:
-  - override /data: im2im/segmentation_plugin.yaml
-  - override /model: im2im/segmentation_plugin.yaml
+  # The data config can be changed to provide instance or semantic segmentations. The model configuration (i.e. number of output channels, loss function) should be updated to match the data.
+  - override /data: im2im/instance_seg.yaml
+  - override /model: im2im/vit_segmentation_decoder.yaml
   - override /callbacks: default.yaml
   - override /trainer: gpu.yaml
-  - override /logger: mlflow.yaml
+  - override /logger: csv.yaml
 
 # all parameters below will be merged with parameters from default configurations set above
 # this allows you to overwrite only specified parameters
 
 tags: ["dev"]
 seed: 12345
 
 experiment_name: YOUR_EXP_NAME
 run_name: YOUR_RUN_NAME
-
-# manifest columns
 source_col: raw
-target_col1: seg1
-target_col2: seg2
-merge_mask_col: merge_mask
-exclude_mask_col: exclude_mask
-base_image_col: base_image
-
-# data params
+target_col: seg
 spatial_dims: 3
-input_channel: 0
+# number of channels in your input images
 raw_im_channels: 1
 
 trainer:
-  max_epochs: 100
+  max_epochs: 1000
 
 data:
-  path: ${paths.data_dir}/example_experiment_data/s3_data
+  path: ${paths.data_dir}/example_experiment_data/segmentation
   cache_dir: ${paths.data_dir}/example_experiment_data/cache
   batch_size: 1
   _aux:
-    patch_shape:
-# small, medium, large
-# 32 pix, 64 pix, 128 pix
-
-# OVERRIDE:
-# data._aux.patch_shape
-# model._aux.strides
-# model._aux.kernel_size
-# model._aux.upsample_kernel_size
+    # 2D
+    # patch_shape: [16, 16]
+    # 3D
+    patch_shape: [16, 16, 16]
```

### Comparing `cyto-dl-0.1.5/configs/experiment/im2im/segmentation_superres.yaml` & `cyto-dl-0.1.6/configs/experiment/im2im/segmentation_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/lattice_nuc_sdf.yaml` & `cyto-dl-0.1.6/configs/experiment/private/lattice_nuc_sdf.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/mnist_so2.yaml` & `cyto-dl-0.1.6/configs/experiment/private/mnist_so2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/npm1_classical_3d_vae.yaml` & `cyto-dl-0.1.6/configs/experiment/private/npm1_classical_3d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/npm1_classical_scale_inv.yaml` & `cyto-dl-0.1.6/configs/experiment/private/npm1_classical_scale_inv.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml` & `cyto-dl-0.1.6/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/npm1_scale_inv_canon_so3.yaml` & `cyto-dl-0.1.6/configs/experiment/private/npm1_scale_inv_canon_so3.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/npm1_so2.yaml` & `cyto-dl-0.1.6/configs/experiment/private/npm1_so2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/npm1_so2_scale_inv.yaml` & `cyto-dl-0.1.6/configs/experiment/private/npm1_so2_scale_inv.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/npm1_so3_scale_inv.yaml` & `cyto-dl-0.1.6/configs/experiment/private/npm1_so3_scale_inv.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/npm1_so3_vae.yaml` & `cyto-dl-0.1.6/configs/experiment/private/npm1_so3_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/npm1_so3_vae_seg.yaml` & `cyto-dl-0.1.6/configs/experiment/private/npm1_so3_vae_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/variance_classical_2d_vae.yaml` & `cyto-dl-0.1.6/configs/experiment/private/variance_classical_2d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/variance_classical_3d_vae.yaml` & `cyto-dl-0.1.6/configs/experiment/private/variance_classical_3d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/variance_so2_3d_vae.yaml` & `cyto-dl-0.1.6/configs/experiment/private/variance_so2_3d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/variance_so2_3d_vae_profiling.yaml` & `cyto-dl-0.1.6/configs/experiment/private/variance_so2_3d_vae_profiling.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/variance_spharm.yaml` & `cyto-dl-0.1.6/configs/experiment/private/variance_spharm.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/experiment/private/variance_spharm_o2.yaml` & `cyto-dl-0.1.6/configs/experiment/private/variance_spharm_o2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/hparams_search/mnist_optuna.yaml` & `cyto-dl-0.1.6/configs/hparams_search/mnist_optuna.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/logger/wandb.yaml` & `cyto-dl-0.1.6/configs/logger/wandb.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/classification/single_timepoint.yaml` & `cyto-dl-0.1.6/configs/model/classification/single_timepoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/im2im/gan.yaml` & `cyto-dl-0.1.6/configs/model/im2im/gan.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/im2im/gan_superres.yaml` & `cyto-dl-0.1.6/configs/model/im2im/gan_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/im2im/instance_seg.yaml` & `cyto-dl-0.1.6/configs/model/im2im/instance_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/im2im/labelfree.yaml` & `cyto-dl-0.1.6/configs/model/im2im/labelfree.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/im2im/mae.yaml` & `cyto-dl-0.1.6/configs/model/im2im/mae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/im2im/segmentation.yaml` & `cyto-dl-0.1.6/configs/model/im2im/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/im2im/segmentation_plugin.yaml` & `cyto-dl-0.1.6/configs/model/im2im/segmentation_plugin.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -6,33 +6,36 @@
 x_key: ${source_col}
 
 backbone:
   _target_: monai.networks.nets.DynUNet
   spatial_dims: ${spatial_dims}
   in_channels: ${raw_im_channels}
   out_channels: 1
-  strides: ${model._aux.strides}
-  kernel_size: ${model._aux.kernel_size}
-  upsample_kernel_size: ${model._aux.upsample_kernel_size}
+  strides: [1, 2, 2]
+  kernel_size: [3, 3, 3]
+  upsample_kernel_size: [2, 2]
   dropout: 0.0
   res_block: True
+  filters: ${model._aux.filters}
 
 task_heads:
   target:
-    _target_: cyto_dl.nn.BaseHead
+    _target_: cyto_dl.nn.head.MaskHead
+    mask_key: ${exclude_mask_col}
     loss:
       _target_: monai.losses.MaskedDiceLoss
       sigmoid: True
     postprocess:
       input:
         _target_: cyto_dl.models.im2im.utils.postprocessing.ActThreshLabel
         rescale_dtype: numpy.uint8
       prediction:
         _target_: cyto_dl.models.im2im.utils.postprocessing.AutoThreshold
         method: "threshold_otsu"
+
     save_input: True
 
 optimizer:
   generator:
     _partial_: True
     _target_: torch.optim.Adam
     lr: 0.0001
@@ -43,14 +46,13 @@
     _partial_: True
     _target_: torch.optim.lr_scheduler.ExponentialLR
     gamma: 0.995
 
 inference_args:
   sw_batch_size: 1
   roi_size: ${data._aux.patch_shape}
-  overlap: 0.25
+  overlap: ${model._aux.overlap}
   mode: "gaussian"
 
 _aux:
-  strides:
-  kernel_size:
-  upsample_kernel_size:
+  filters:
+  overlap:
```

### Comparing `cyto-dl-0.1.5/configs/model/im2im/segmentation_superres.yaml` & `cyto-dl-0.1.6/configs/model/im2im/segmentation_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/im2im/vit_segmentation_decoder.yaml` & `cyto-dl-0.1.6/configs/model/im2im/vit_segmentation_decoder.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/private/classical_image_vae.yaml` & `cyto-dl-0.1.6/configs/model/private/classical_image_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/private/spharm.yaml` & `cyto-dl-0.1.6/configs/model/private/spharm.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/test/base.yaml` & `cyto-dl-0.1.6/configs/model/test/base.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/model/test/simple_segmentation.yaml` & `cyto-dl-0.1.6/configs/model/test/simple_segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/configs/train.yaml` & `cyto-dl-0.1.6/configs/train.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/api/data.py` & `cyto-dl-0.1.6/cyto_dl/api/data.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/api/model.py` & `cyto-dl-0.1.6/cyto_dl/api/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from cyto_dl.eval import evaluate
 from cyto_dl.train import train as train_model
 from cyto_dl.utils.download_test_data import download_test_data
 from cyto_dl.utils.rich_utils import print_config_tree
 
 
 class CytoDLModel:
+    # TODO: add optional CytoDLConfig param to init--if client passes a
+    # CytoDLConfig subtype, config will be initialized in constructor and
+    # calls to train/predict can be run immediately
     def __init__(self):
         self.cfg = None
         self._training = False
         self._predicting = False
 
         self.root = pyrootutils.setup_root(
             search_from=__file__,
```

### Comparing `cyto-dl-0.1.5/cyto_dl/callbacks/callback_utils.py` & `cyto-dl-0.1.6/cyto_dl/callbacks/callback_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/callbacks/latent_walk.py` & `cyto-dl-0.1.6/cyto_dl/callbacks/latent_walk.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/callbacks/layer_freeze.py` & `cyto-dl-0.1.6/cyto_dl/callbacks/layer_freeze.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/callbacks/model_utils.py` & `cyto-dl-0.1.6/cyto_dl/callbacks/model_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/callbacks/outlier_detection.py` & `cyto-dl-0.1.6/cyto_dl/callbacks/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/compile.py` & `cyto-dl-0.1.6/cyto_dl/compile.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/dataframe/readers.py` & `cyto-dl-0.1.6/cyto_dl/dataframe/readers.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/dataframe/transforms/filter.py` & `cyto-dl-0.1.6/cyto_dl/dataframe/transforms/filter.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/dataframe/transforms/group_cols.py` & `cyto-dl-0.1.6/cyto_dl/dataframe/transforms/group_cols.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/dataframe/transforms/misc.py` & `cyto-dl-0.1.6/cyto_dl/dataframe/transforms/misc.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/dataframe/transforms/split.py` & `cyto-dl-0.1.6/cyto_dl/dataframe/transforms/split.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/datamodules/czi.py` & `cyto-dl-0.1.6/cyto_dl/datamodules/czi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Callable, Optional, Union
 
 import numpy as np
 import pandas as pd
-from aicsimageio.aics_image import AICSImage
+from bioio import BioImage
 from monai.data import DataLoader, Dataset, MetaTensor
 from monai.transforms import Compose, apply_transform
 from omegaconf import ListConfig
 
 
 class CZIDataset(Dataset):
     """Dataset converting a `.csv` file listing CZI files and some metadata into batches of single-
@@ -95,15 +95,15 @@
             timepoints = list(range(img.dims.T))
         return timepoints
 
     def get_per_file_args(self, df):
         img_data = []
         for row in df.itertuples():
             row = row._asdict()
-            img = AICSImage(row[self.img_path_column])
+            img = BioImage(row[self.img_path_column])
             scenes = self._get_scenes(row, img)
             timepoints = self._get_timepoints(row, img)
             for scene in scenes:
                 for timepoint in timepoints:
                     img_data.append(
                         {
                             "img": img,
```

### Comparing `cyto-dl-0.1.5/cyto_dl/datamodules/data_dict.py` & `cyto-dl-0.1.6/cyto_dl/datamodules/data_dict.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/dataframe_datamodule.py` & `cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/dataframe_datamodule.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py` & `cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/utils.py` & `cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/datamodules/folder.py` & `cyto-dl-0.1.6/cyto_dl/datamodules/folder.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/datamodules/smartcache.py` & `cyto-dl-0.1.6/cyto_dl/datamodules/smartcache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import dask
 import numpy as np
 import pandas as pd
-from aicsimageio import AICSImage
+from bioio import BioImage
 from dask.diagnostics import ProgressBar
 from lightning import LightningDataModule
 from monai.data import DataLoader
 from monai.data.dataset import CacheDataset, Dataset, SmartCacheDataset
 from monai.transforms import Compose
 from sklearn.model_selection import train_test_split
 
@@ -34,15 +34,15 @@
     ):
         """
         Parameters
         ----------
         csv_path: Union[Path, str]
             path to csv with image in `img_path_column` and channel in `channel_column`
         transforms: Compose
-            Monai transforms to apply to each image. Should start with a transform that uses AICSimageio for image reading
+            Monai transforms to apply to each image. Should start with a transform that uses bioio for image reading
         img_data: Union[Path, str]
             csv_path generated by get_per_file_args that enumerates scenes and timepoints for each image in csv_path
         n_val: int
             number of validation images to use. Minimum of pct_val * n_images and n_val is used.
         pct_val: float
             percentage of images to use for validation. Minimum of pct_val * n_images and n_val is used.
         img_path_column: str
@@ -105,15 +105,15 @@
         if self.num_neighbors > 0:
             return timepoints[: -self.num_neighbors]
         return timepoints
 
     @dask.delayed
     def _get_file_args(self, row):
         row = row._asdict()
-        img = AICSImage(row[self.img_path_column])
+        img = BioImage(row[self.img_path_column])
         scenes = self._get_scenes(img)
         timepoints = self._get_timepoints(img)
         img_data = []
         use_neighbors = self.num_neighbors > 0
         for scene in scenes:
             for timepoint in timepoints:
                 img_data.append(
```

### Comparing `cyto-dl-0.1.5/cyto_dl/datamodules/torchvision.py` & `cyto-dl-0.1.6/cyto_dl/datamodules/torchvision.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/eval.py` & `cyto-dl-0.1.6/cyto_dl/eval.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/io/aicsimage_loader.py` & `cyto-dl-0.1.6/cyto_dl/image/io/aicsimage_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 import numpy as np
-from aicsimageio import AICSImage
+from bioio import BioImage
 from monai.data import MetaTensor
 from monai.transforms import Transform
 
 
 class AICSImageLoaderd(Transform):
     """Enumerates scenes and timepoints for dictionary with format.
 
@@ -28,15 +28,15 @@
         Parameters
         ----------
         path_key : str = "path"
             Key for the path to the image
         scene_key : str = "scene"
             Key for the scene number
         kwargs_keys : List = ["dimension_order_out", "C", "T"]
-            Keys for the kwargs to pass to AICSImage.get_image_dask_data
+            Keys for the kwargs to pass to BioImage.get_image_dask_data
         out_key : str = "raw"
             Key for the output image
         allow_missing_keys : bool = False
             Whether to allow missing keys in the data dictionary
         dask_load: bool = True
             Whether to use dask to load images. If False, full images are loaded into memory before extracting specified scenes/timepoints.
         """
@@ -51,15 +51,15 @@
 
     def __call__(self, data):
         # copying prevents the dataset from being modified inplace - important when using partially cached datasets so that the memory use doesn't increase over time
         data = data.copy()
         if self.path_key not in data and not self.allow_missing_keys:
             raise KeyError(f"Missing key {self.path_key} in data dictionary")
         path = data[self.path_key]
-        img = AICSImage(path)
+        img = BioImage(path)
         if self.scene_key in data:
             img.set_scene(data[self.scene_key])
         kwargs = {k: data[k] for k in self.kwargs_keys}
         if self.dask_load:
             img = img.get_image_dask_data(**kwargs).compute()
         else:
             img = img.get_image_data(**kwargs)
```

### Comparing `cyto-dl-0.1.5/cyto_dl/image/io/monai_bio_reader.py` & `cyto-dl-0.1.6/cyto_dl/image/io/monai_bio_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """ADAPTED FROM https://github.com/MMV-Lab/mmv_im2im/"""
 
 from typing import Dict, List, Sequence, Tuple, Union
 
 import numpy as np
-from aicsimageio import AICSImage
+from bioio import BioImage
 from monai.config import PathLike
 from monai.data import ImageReader
 from monai.data.image_reader import _stack_images
 from monai.utils import ensure_tuple, require_pkg
 from omegaconf import Container, OmegaConf
 
 
-@require_pkg(pkg_name="aicsimageio")
+@require_pkg(pkg_name="bioio")
 class MonaiBioReader(ImageReader):
     def __init__(self, dask_load: bool = True, **reader_kwargs):
         """
         dask_load: bool = True
             Whether to use dask to load images. If False, full images are loaded into memory before extracting specified scenes/timepoints.
         reader_kwargs: Dict
-            Additional keyword arguments to pass to AICSImage.get_image_data or AICSImage.get_image_dask_data
+            Additional keyword arguments to pass to BioImage.get_image_data or BioImage.get_image_dask_data
         """
         super().__init__()
         self.reader_kwargs = {
             k: OmegaConf.to_container(v) if isinstance(v, Container) else v
             for k, v in reader_kwargs.items()
             if v is not None
         }
         self.dask_load = dask_load
 
     def read(self, data: Union[Sequence[PathLike], PathLike]):
         filenames: Sequence[PathLike] = ensure_tuple(data)
         img_ = []
         for name in filenames:
-            img_.append(AICSImage(f"{name}"))
+            img_.append(BioImage(f"{name}"))
 
         return img_ if len(filenames) > 1 else img_[0]
 
     def get_data(self, img) -> Tuple[np.ndarray, Dict]:
         img_array: List[np.ndarray] = []
 
         for img_obj in ensure_tuple(img):
```

### Comparing `cyto-dl-0.1.5/cyto_dl/image/io/numpy_reader.py` & `cyto-dl-0.1.6/cyto_dl/image/io/numpy_reader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/io/ome_zarr_reader.py` & `cyto-dl-0.1.6/cyto_dl/image/io/ome_zarr_reader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/io/polygon_loader.py` & `cyto-dl-0.1.6/cyto_dl/image/io/polygon_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 
                 mask_shape = input_dict[self.shape_reference_key].shape[-2:]
                 mask = np.zeros(mask_shape)
                 for p in poly:
                     mask = np.logical_or(mask, polygon2mask(mask_shape, p))
                 if self.propagate_3d:
                     mask = np.stack([mask] * input_dict[self.shape_reference_key].shape[1])
+                # all ones except for regions in polygon
+                mask = ~mask
                 input_dict[key] = np.expand_dims(mask > 0, 0)
             elif self.missing_key_mode == "raise":
                 raise KeyError(
                     f"key `{key}` not available. Available keys are {input_dict.keys()}"
                 )
             elif self.missing_key_mode == "create":
                 input_dict[key] = np.ones_like(input_dict[self.shape_reference_key])
```

### Comparing `cyto-dl-0.1.5/cyto_dl/image/io/skimage_reader.py` & `cyto-dl-0.1.6/cyto_dl/image/io/skimage_reader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/__init__.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/bright_sampler.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/bright_sampler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/clip.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/clip.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/contrastadjust.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/contrastadjust.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/merge.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 from typing import Union
 
 from monai.transforms import Transform
 
 
 class Merged(Transform):
     """Use mask to merge two images."""
@@ -34,37 +35,44 @@
     def __call__(self, input_dict):
         """
         Parameters
         ----------
         input_dict: Dict[str, torch.Tensor]
             dict of CZYX tensors/metadata/paths
         """
-        # no merging mask, return original dict
-        if self.mask_key not in input_dict or input_dict[self.mask_key] is None:
-            return input_dict
-
-        mask = input_dict[self.mask_key]
-
         if self.base_image_key not in input_dict:
             raise KeyError(
                 f"key `{self.base_image_key}` not available. Available keys are {input_dict.keys()}"
             )
         base_image_name = input_dict[self.base_image_key]
 
         if base_image_name not in self.image_keys:
             raise KeyError(
                 f"Base image name `{base_image_name}` must match provided image keys `{self.image_keys}`"
             )
 
+        if self.mask_key not in input_dict or input_dict[self.mask_key] is None:
+            # no merging mask, return original dict
+            input_dict[self.output_name] = deepcopy(input_dict[base_image_name])
+            # remove mask key if it exists
+            input_dict.pop(self.mask_key, None)
+            return input_dict
+
+        mask = input_dict[self.mask_key].astype(bool)
+        # From polygoan loader, 1 is everything outside of the polygon, 0 inside the polygon.
+        # For merging we want to inver this
+        mask = ~mask
+
         for key in self.image_keys:
             if key not in input_dict.keys():
                 raise KeyError(
                     f"key `{key}` not available. Available keys are {input_dict.keys()}"
                 )
 
         base_image = input_dict[base_image_name]
-        self.image_keys.remove(base_image_name)
-        merge_image = input_dict[self.image_keys[0]]
+        merge_image = input_dict[
+            self.image_keys[0] if self.image_keys[1] == base_image_name else self.image_keys[1]
+        ]
 
         input_dict[self.output_name] = (base_image * ~mask) + (merge_image * mask)
 
         return input_dict
```

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/multiscale_cropper.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/multiscale_cropper.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/pad.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/project.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/project.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/rotation_mask_transform.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/rotation_mask_transform.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/save.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/save.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Sequence, Union
 
 import numpy as np
 import torch
-from aicsimageio.writers import OmeTiffWriter
+from bioio.writers import OmeTiffWriter
 from monai.data.meta_tensor import MetaTensor
 from monai.transforms import Transform
 from omegaconf import ListConfig
 
 
 class Save(Transform):
     def __init__(
```

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/so2_random_rotation.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/so2_random_rotation.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/image/transforms/track_transforms.py` & `cyto-dl-0.1.6/cyto_dl/image/transforms/track_transforms.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/loggers/mlflow.py` & `cyto-dl-0.1.6/cyto_dl/loggers/mlflow.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/base_model.py` & `cyto-dl-0.1.6/cyto_dl/models/base_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/basic_model.py` & `cyto-dl-0.1.6/cyto_dl/models/basic_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/classification/classification.py` & `cyto-dl-0.1.6/cyto_dl/models/classification/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import torch
 import torch.nn as nn
-from aicsimageio.writers import OmeTiffWriter
+from bioio.writers import OmeTiffWriter
 from PIL import Image, ImageDraw, ImageFont
 from skimage.exposure import rescale_intensity
 from torchmetrics import MeanMetric
 from torchmetrics.classification import MulticlassF1Score
 
 from cyto_dl.models.base_model import BaseModel
```

### Comparing `cyto-dl-0.1.5/cyto_dl/models/classification/timepoint_classification.py` & `cyto-dl-0.1.6/cyto_dl/models/classification/timepoint_classification.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/handlers/base_handler.py` & `cyto-dl-0.1.6/cyto_dl/models/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/handlers/image_handler.py` & `cyto-dl-0.1.6/cyto_dl/models/handlers/image_handler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/handlers/load_image_patch.py` & `cyto-dl-0.1.6/cyto_dl/models/handlers/load_image_patch.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/im2im/gan.py` & `cyto-dl-0.1.6/cyto_dl/models/im2im/gan.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/im2im/multi_task.py` & `cyto-dl-0.1.6/cyto_dl/models/im2im/multi_task.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/instance_seg.py` & `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/instance_seg.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/noise_annealer.py` & `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/noise_annealer.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py` & `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py` & `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import importlib
 from typing import Optional, Union
 
+import numpy as np
+
 
 class AutoThreshold:
     def __init__(self, method: Optional[Union[float, str]] = None):
         if isinstance(method, float):
 
             def thresh_func(image):
                 return method
@@ -17,10 +19,11 @@
         elif method is None:
             thresh_func = None
         else:
             raise TypeError("method must be a float or a string")
         self.thresh_func = thresh_func
 
     def __call__(self, image):
+        image = image.detach().cpu().float().numpy()
         if self.thresh_func is None:
             return image
-        return image > self.thresh_func(image)
+        return (image > self.thresh_func(image)).astype(np.uint8)
```

### Comparing `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py` & `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/utils/mlflow.py` & `cyto-dl-0.1.6/cyto_dl/models/utils/mlflow.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/base_vae.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/base_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/image_canon_vae.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/image_canon_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/image_encoder.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/image_encoder.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/image_vae.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/image_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/latent_loss_vae.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/latent_loss_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/point_cloud_vae.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/point_cloud_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/priors/abstract_prior.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/priors/abstract_prior.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/priors/gaussian.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/priors/gaussian.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/priors/joint_prior.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/priors/joint_prior.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/models/vae/tabular_vae.py` & `cyto-dl-0.1.6/cyto_dl/models/vae/tabular_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/discriminators/multi_scale_discriminator.py` & `cyto-dl-0.1.6/cyto_dl/nn/discriminators/multi_scale_discriminator.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/discriminators/n_layer_discriminator.py` & `cyto-dl-0.1.6/cyto_dl/nn/discriminators/n_layer_discriminator.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/head/base_head.py` & `cyto-dl-0.1.6/cyto_dl/nn/head/base_head.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC
 from pathlib import Path
 
 import torch
-from aicsimageio.writers import OmeTiffWriter
+from bioio.writers import OmeTiffWriter
 
 from cyto_dl.models.im2im.utils.postprocessing import detach
 
 
 class BaseHead(ABC, torch.nn.Module):
     """Base class for task heads."""
```

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/head/gan_head.py` & `cyto-dl-0.1.6/cyto_dl/nn/head/gan_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/head/gan_head_superres.py` & `cyto-dl-0.1.6/cyto_dl/nn/head/gan_head_superres.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/head/mae_head.py` & `cyto-dl-0.1.6/cyto_dl/nn/head/mae_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/head/mask_head.py` & `cyto-dl-0.1.6/cyto_dl/nn/head/mask_head.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,18 @@
         postprocess={"input": detach, "prediction": detach}
             Postprocessing for `input` and `predictions` of head
         calculate_metric=False
             Whether to calculate a metric during training. Not used by GAN head.
         save_input=False
             Whether to save out example input images during training
         """
-        super().__init__()
-        self.loss = loss
-        self.postprocess = postprocess
+        super().__init__(loss, postprocess=postprocess, save_input=save_input)
         self.mask_key = mask_key
 
         self.model = torch.nn.Sequential(torch.nn.Identity())
-        self.save_input = save_input
 
     def _calculate_loss(self, y_hat, y, mask):
         return self.loss(y_hat, y, mask)
 
     def run_head(
         self,
         backbone_features,
```

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/head/res_blocks_head.py` & `cyto-dl-0.1.6/cyto_dl/nn/head/res_blocks_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/hr_skip.py` & `cyto-dl-0.1.6/cyto_dl/nn/hr_skip.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/__init__.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/adversarial_loss.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/chamfer_loss.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/chamfer_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/continuous_bernoulli.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/continuous_bernoulli.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/cosine_loss.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/cosine_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/gan_loss.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/gan_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/gaussian_nll_loss.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/gaussian_nll_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/geomloss.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/geomloss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/loss_wrapper.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/loss_wrapper.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/spharm_loss.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/spharm_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/threshold_loss.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/threshold_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/weibull.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/weibull.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/losses/weighted_mse_loss.py` & `cyto-dl-0.1.6/cyto_dl/nn/losses/weighted_mse_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/mlp.py` & `cyto-dl-0.1.6/cyto_dl/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/point_cloud/dgcnn.py` & `cyto-dl-0.1.6/cyto_dl/nn/point_cloud/dgcnn.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/point_cloud/folding_net.py` & `cyto-dl-0.1.6/cyto_dl/nn/point_cloud/folding_net.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/point_cloud/graph_functions.py` & `cyto-dl-0.1.6/cyto_dl/nn/point_cloud/graph_functions.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/point_cloud/vnn.py` & `cyto-dl-0.1.6/cyto_dl/nn/point_cloud/vnn.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/res_unit.py` & `cyto-dl-0.1.6/cyto_dl/nn/res_unit.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/spatial_transformer.py` & `cyto-dl-0.1.6/cyto_dl/nn/spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/track_sequence_predictor.py` & `cyto-dl-0.1.6/cyto_dl/nn/track_sequence_predictor.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/cross_attention.py` & `cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/cross_attention.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/intermediate_weigher.py` & `cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/intermediate_weigher.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/patchify.py` & `cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/patchify.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/vits/cross_mae.py` & `cyto-dl-0.1.6/cyto_dl/nn/vits/cross_mae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/vits/mae.py` & `cyto-dl-0.1.6/cyto_dl/nn/vits/mae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/nn/vits/seg.py` & `cyto-dl-0.1.6/cyto_dl/nn/vits/seg.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/point_cloud/io/read_pcloud.py` & `cyto-dl-0.1.6/cyto_dl/point_cloud/io/read_pcloud.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/train.py` & `cyto-dl-0.1.6/cyto_dl/train.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/utils/config.py` & `cyto-dl-0.1.6/cyto_dl/utils/config.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/utils/download_test_data.py` & `cyto-dl-0.1.6/cyto_dl/utils/download_test_data.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/utils/dummy_dataset.py` & `cyto-dl-0.1.6/cyto_dl/utils/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/utils/pylogger.py` & `cyto-dl-0.1.6/cyto_dl/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/utils/rich_utils.py` & `cyto-dl-0.1.6/cyto_dl/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/utils/rotation.py` & `cyto-dl-0.1.6/cyto_dl/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/utils/spharm/reconstruction.py` & `cyto-dl-0.1.6/cyto_dl/utils/spharm/reconstruction.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/utils/spharm/rotation.py` & `cyto-dl-0.1.6/cyto_dl/utils/spharm/rotation.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/cyto_dl/utils/template_utils.py` & `cyto-dl-0.1.6/cyto_dl/utils/template_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/pyproject.toml` & `cyto-dl-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,55 +3,55 @@
     "pdm-pep517>=1.0.0",
     "numpy>=1.23.5",
 ]
 build-backend = "pdm.pep517.api"
 
 [project]
 name = "cyto-dl"
-version = "0.1.5"
+version = "0.1.6"
 description = "Collection of representation learning models, techniques, callbacks, utils, used to create latent variable models of cell shape, morphology and intracellular organization."
 readme = "README.md"
 authors = [
     { name = "Benji Morris", email = "benjamin.morris@alleninstitute.org" },
     { name = "Guilherme Pires", email = "guilherme.pires@alleninstitute.org" },
     { name = "Ritvik Vasan", email = "ritvik.vasan@alleninstitute.org" },
 ]
 dependencies = [
-    "hydra-core~=1.3",
-    "hydra-colorlog~=1.2",
-    "hydra-optuna-sweeper~=1.2",
-    "torch>=2.0,<2.1",
-    "numpy~=1.23",
-    "matplotlib~=3.7",
-    "pandas~=1.5",
-    "fire~=0.5",
-    "joblib~=1.2",
-    "mlflow~=2.1",
-    "omegaconf~=2.3",
-    "pyarrow~=10.0",
-    "pyrootutils~=1.0",
-    "PyYAML~=6.0",
-    "scikit-learn~=1.2",
-    "aicsimageio~=4.11.0",
-    "universal-pathlib~=0.0",
-    "ome-zarr~=0.6",
-    "anndata~=0.8",
-    "bfio==2.3.0",
+    "hydra-core~=1.3.0",
+    "hydra-colorlog>=1.2",
+    "hydra-optuna-sweeper>=1.2",
+    "torch~=2.0.0",
+    "numpy>=1.23",
+    "matplotlib>=3.7",
+    "pandas>=1.5",
+    "fire>=0.5",
+    "mlflow>=2.1",
+    "omegaconf>=2.3",
+    "pyarrow>=10.0",
+    "pyrootutils>=1.0",
+    "PyYAML>=6.0",
+    "scikit-learn>=1.2",
+    "universal-pathlib>=0.0",
+    "ome-zarr>=0.6",
+    "anndata>=0.8",
     "monai-weekly>=1.2.dev2308",
-    "tifffile~=2023.2",
     "timm>=0.9.7",
-    "tqdm~=4.64",
-    "protobuf<=3.20.1",
-    "lightning>=2.0,<2.1",
-    "ostat>=0.2",
+    "tqdm>=4.64",
+    "lightning>=2.0",
     "einops>=0.6.1",
     "edt>=2.3.1",
-    "astropy~=5.2",
+    "astropy>=5.2",
+    "rich",
+    "boto3",
+    "bioio",
+    "bioio-czi",
+    "bioio-ome-tiff",
+    "bioio-tifffile",
 ]
-requires-python = ">=3.8,<3.11"
+requires-python = ">=3.9,<3.11"
 
 [project.optional-dependencies]
 equiv = [
     "lie_learn==0.0.1.post1",
     "escnn~=1.0.7",
     "py3nj==0.1.2",
     "e3nn~=0.5.1",
```

### Comparing `cyto-dl-0.1.5/tests/api/test_model.py` & `cyto-dl-0.1.6/tests/api/test_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/conftest.py` & `cyto-dl-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/helpers/package_available.py` & `cyto-dl-0.1.6/tests/helpers/package_available.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/helpers/run_if.py` & `cyto-dl-0.1.6/tests/helpers/run_if.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/resources/rand_im.tif` & `cyto-dl-0.1.6/tests/resources/rand_im.tif`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/resources/train.csv` & `cyto-dl-0.1.6/tests/resources/train.csv`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/test_alternating_batch_sampler.py` & `cyto-dl-0.1.6/tests/test_alternating_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/test_configs.py` & `cyto-dl-0.1.6/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/test_eval.py` & `cyto-dl-0.1.6/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/test_mlflow_logger.py` & `cyto-dl-0.1.6/tests/test_mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/test_polygon_loader.py` & `cyto-dl-0.1.6/tests/test_polygon_loader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/tests/test_train.py` & `cyto-dl-0.1.6/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.5/PKG-INFO` & `cyto-dl-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cyto-dl
-Version: 0.1.5
+Version: 0.1.6
 Summary: Collection of representation learning models, techniques, callbacks, utils, used to create latent variable models of cell shape, morphology and intracellular organization.
 Author-email: Benji Morris <benjamin.morris@alleninstitute.org>,Guilherme Pires <guilherme.pires@alleninstitute.org>,Ritvik Vasan <ritvik.vasan@alleninstitute.org>
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.11
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: equiv
 Provides-Extra: pcloud
 Provides-Extra: s3
 Provides-Extra: spharm
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: cyto-dl Version: 0.1.5 Summary: Collection of
+Metadata-Version: 2.1 Name: cyto-dl Version: 0.1.6 Summary: Collection of
 representation learning models, techniques, callbacks, utils, used to create
 latent variable models of cell shape, morphology and intracellular
 organization. Author-email: Benji Morris
 alleninstitute.org>,Guilherme Pires
 alleninstitute.org>,Ritvik Vasan
-alleninstitute.org> Requires-Python: >=3.8,<3.11 Provides-Extra: all Provides-
+alleninstitute.org> Requires-Python: >=3.9,<3.11 Provides-Extra: all Provides-
 Extra: docs Provides-Extra: equiv Provides-Extra: pcloud Provides-Extra: s3
 Provides-Extra: spharm Provides-Extra: test Provides-Extra: torchserve Project-
 URL: Homepage, https://github.com/AllenCellModeling/cyto-dl Description-
 Content-Type: text/markdown
                              ************ CCyyttooDDLL ************
                  _[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_C_o_n_f_i_g_:_ _H_y_d_r_a_]_[_T_e_m_p_l_a_t_e_]
               [https://github.com/AllenCellModeling/cyto-dl/blob/
```

