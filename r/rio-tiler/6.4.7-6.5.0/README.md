# Comparing `tmp/rio_tiler-6.4.7.tar.gz` & `tmp/rio_tiler-6.5.0.tar.gz`

## Comparing `rio_tiler-6.4.7.tar` & `rio_tiler-6.5.0.tar`

### file list

```diff
@@ -1,241 +1,241 @@
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/__init__.py
--rw-r--r--   0        0        0     9775 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/colormap.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/constants.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/errors.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/expression.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/logger.py
--rw-r--r--   0        0        0    28149 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/models.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/py.typed
--rw-r--r--   0        0        0    21841 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/reader.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/tasks.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/types.py
--rw-r--r--   0        0        0    27257 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/utils.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/accent.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/accent_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/afmhot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/afmhot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/algae.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/algae_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/amp.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/amp_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/autumn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/autumn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/balance.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/balance_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/binary.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/binary_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/blues.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/blues_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/bone.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/bone_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/brbg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/brbg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/brg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/brg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/bugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/bugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/bupu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/bupu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/bwr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/bwr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/cfastie.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/cividis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/cividis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/cmrmap.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/cmrmap_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/cool.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/cool_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/coolwarm.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/coolwarm_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/copper.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/copper_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/cubehelix.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/cubehelix_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/curl.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/curl_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/dark2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/dark2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/deep.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/deep_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/delta.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/delta_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/dense.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/dense_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/diff.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/diff_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/flag.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/flag_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_earth.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_earth_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_heat.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_heat_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_ncar.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_ncar_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_stern.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_stern_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_yarg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gist_yarg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gnuplot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gnuplot2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gnuplot2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gnuplot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/greens.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/greens_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/greys.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/greys_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/haline.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/haline_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/hot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/hot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/hsv.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/hsv_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ice.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ice_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/inferno.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/inferno_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/jet.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/jet_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/magma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/magma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/matter.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/matter_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/nipy_spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/nipy_spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ocean.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ocean_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/oranges.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/oranges_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/orrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/orrd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/oxy.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/oxy_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/paired.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/paired_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pastel1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pastel1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pastel2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pastel2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/phase.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/phase_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pink.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pink_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/piyg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/piyg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/plasma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/plasma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/prgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/prgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/prism.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/prism_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pubu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pubu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pubugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/pubugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/puor.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/puor_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/purd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/purd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/purples.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/purples_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rain.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rain_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdgy.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdgy_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdpu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdpu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdylbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdylbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rdylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/reds.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/reds_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/rplumbo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/schwarzwald.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/seismic.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/seismic_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/set1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/set1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/set2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/set2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/set3.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/set3_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/solar.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/solar_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/speed.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/speed_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/spring.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/spring_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/summer.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/summer_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tab10.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tab10_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tab20.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tab20_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tab20b.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tab20b_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tab20c.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tab20c_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tarn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tarn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tempo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/tempo_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/terrain.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/terrain_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/thermal.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/thermal_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/topo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/topo_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/turbid.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/turbid_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/turbo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/turbo_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/twilight.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/twilight_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/twilight_shifted.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/twilight_shifted_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/viridis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/viridis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/winter.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/winter_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/wistia.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/wistia_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ylgnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ylgnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ylorbr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ylorbr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ylorrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/cmap_data/ylorrd_r.npy
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/io/__init__.py
--rw-r--r--   0        0        0    45645 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/io/base.py
--rw-r--r--   0        0        0    32154 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/io/rasterio.py
--rw-r--r--   0        0        0    10539 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/io/stac.py
--rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/io/xarray.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/mosaic/__init__.py
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/mosaic/reader.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/mosaic/methods/__init__.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/mosaic/methods/base.py
--rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/rio_tiler/mosaic/methods/defaults.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/.gitignore
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/AUTHORS.txt
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/LICENSE
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/README.md
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/pyproject.toml
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 rio_tiler-6.4.7/PKG-INFO
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/__init__.py
+-rw-r--r--   0        0        0     9775 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/colormap.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/constants.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/errors.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/expression.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/logger.py
+-rw-r--r--   0        0        0    28149 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/models.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/py.typed
+-rw-r--r--   0        0        0    21927 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/reader.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/tasks.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/types.py
+-rw-r--r--   0        0        0    27748 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/utils.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/accent.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/accent_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/afmhot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/afmhot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/algae.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/algae_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/amp.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/amp_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/autumn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/autumn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/balance.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/balance_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/binary.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/binary_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/blues.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/blues_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/bone.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/bone_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/brbg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/brbg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/brg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/brg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/bugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/bugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/bupu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/bupu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/bwr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/bwr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/cfastie.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/cividis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/cividis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/cmrmap.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/cmrmap_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/cool.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/cool_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/coolwarm.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/coolwarm_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/copper.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/copper_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/cubehelix.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/cubehelix_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/curl.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/curl_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/dark2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/dark2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/deep.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/deep_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/delta.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/delta_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/dense.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/dense_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/diff.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/diff_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/flag.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/flag_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_earth.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_earth_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_heat.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_heat_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_ncar.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_ncar_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_stern.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_stern_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_yarg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gist_yarg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gnuplot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gnuplot2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gnuplot2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gnuplot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/greens.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/greens_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/greys.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/greys_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/haline.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/haline_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/hot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/hot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/hsv.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/hsv_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ice.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ice_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/inferno.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/inferno_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/jet.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/jet_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/magma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/magma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/matter.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/matter_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/nipy_spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/nipy_spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ocean.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ocean_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/oranges.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/oranges_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/orrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/orrd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/oxy.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/oxy_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/paired.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/paired_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pastel1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pastel1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pastel2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pastel2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/phase.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/phase_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pink.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pink_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/piyg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/piyg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/plasma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/plasma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/prgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/prgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/prism.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/prism_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pubu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pubu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pubugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/pubugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/puor.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/puor_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/purd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/purd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/purples.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/purples_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rain.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rain_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdgy.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdgy_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdpu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdpu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdylbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdylbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rdylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/reds.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/reds_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/rplumbo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/schwarzwald.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/seismic.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/seismic_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/set1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/set1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/set2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/set2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/set3.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/set3_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/solar.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/solar_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/speed.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/speed_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/spring.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/spring_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/summer.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/summer_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tab10.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tab10_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tab20.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tab20_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tab20b.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tab20b_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tab20c.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tab20c_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tarn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tarn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tempo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/tempo_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/terrain.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/terrain_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/thermal.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/thermal_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/topo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/topo_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/turbid.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/turbid_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/turbo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/turbo_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/twilight.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/twilight_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/twilight_shifted.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/twilight_shifted_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/viridis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/viridis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/winter.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/winter_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/wistia.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/wistia_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ylgnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ylgnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ylorbr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ylorbr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ylorrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/cmap_data/ylorrd_r.npy
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/io/__init__.py
+-rw-r--r--   0        0        0    45645 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/io/base.py
+-rw-r--r--   0        0        0    32154 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/io/rasterio.py
+-rw-r--r--   0        0        0    10539 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/io/stac.py
+-rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/io/xarray.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/mosaic/__init__.py
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/mosaic/reader.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/mosaic/methods/__init__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/mosaic/methods/base.py
+-rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/rio_tiler/mosaic/methods/defaults.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/.gitignore
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/AUTHORS.txt
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/LICENSE
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/README.md
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 rio_tiler-6.5.0/PKG-INFO
```

### Comparing `rio_tiler-6.4.7/rio_tiler/colormap.py` & `rio_tiler-6.5.0/rio_tiler/colormap.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/errors.py` & `rio_tiler-6.5.0/rio_tiler/errors.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/expression.py` & `rio_tiler-6.5.0/rio_tiler/expression.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/models.py` & `rio_tiler-6.5.0/rio_tiler/models.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/profiles.py` & `rio_tiler-6.5.0/rio_tiler/profiles.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/reader.py` & `rio_tiler-6.5.0/rio_tiler/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,16 @@
 
     # Use WarpedVRT when Re-projection or User VRT Option (cutline)
     if (dst_crs != src_dst.crs) or vrt_options:
         window = None
         vrt_transform, vrt_width, vrt_height = get_vrt_transform(
             src_dst,
             bounds,
+            height,
+            width,
             dst_crs=dst_crs,
             align_bounds_with_dataset=align_bounds_with_dataset,
         )
         bounds = array_bounds(vrt_height, vrt_width, vrt_transform)
 
         if max_size and not (width and height):
             height, width = _get_width_height(max_size, vrt_height, vrt_width)
@@ -380,14 +382,16 @@
         if buffer:
             bounds, height, width = _apply_buffer(buffer, bounds, height, width)
 
             # re-calculate the transform given the new bounds, height and width
             vrt_transform, vrt_width, vrt_height = get_vrt_transform(
                 src_dst,
                 bounds,
+                height,
+                width,
                 dst_crs=dst_crs,
                 align_bounds_with_dataset=align_bounds_with_dataset,
             )
             bounds = array_bounds(vrt_height, vrt_width, vrt_transform)
 
         if padding > 0 and not is_aligned(src_dst, bounds, bounds_crs=dst_crs):
             vrt_transform = vrt_transform * Affine.translation(-padding, -padding)
```

### Comparing `rio_tiler-6.4.7/rio_tiler/tasks.py` & `rio_tiler-6.5.0/rio_tiler/tasks.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/types.py` & `rio_tiler-6.5.0/rio_tiler/types.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/utils.py` & `rio_tiler-6.5.0/rio_tiler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,16 +292,16 @@
     align_bounds_with_dataset: bool = False,
 ) -> Tuple[Affine, int, int]:
     """Calculate VRT transform.
 
     Args:
         src_dst (rasterio.io.DatasetReader or rasterio.io.DatasetWriter or rasterio.vrt.WarpedVRT): Rasterio dataset.
         bounds (tuple): Bounding box coordinates in target crs (**dst_crs**).
-        height (int, optional): Desired output height of the array for the input bounds.
-        width (int, optional): Desired output width of the array for the input bounds.
+        height (int, optional): Output height of the array for the input bounds.
+        width (int, optional): Output width of the array for the input bounds.
         dst_crs (rasterio.crs.CRS, optional): Target Coordinate Reference System. Defaults to `epsg:3857`.
         align_bounds_with_dataset (bool): Align input bounds with dataset transform. Defaults to `False`.
 
     Returns:
         tuple: VRT transform (affine.Affine), width (int) and height (int)
 
     """
@@ -380,39 +380,43 @@
 
     elif align_bounds_with_dataset:
         window = _round_window(windows.from_bounds(*bounds, transform=dst_transform))
         bounds = windows.bounds(window, dst_transform)
 
     w, s, e, n = bounds
 
-    # TODO: Explain
-    if not height or not width:
-        vrt_width = max(1, round((e - w) / dst_transform.a))
-        vrt_height = max(1, round((s - n) / dst_transform.e))
-        vrt_transform = from_bounds(w, s, e, n, vrt_width, vrt_height)
-        return vrt_transform, vrt_width, vrt_height
-
-    # TODO: Explain
-    tile_transform = from_bounds(w, s, e, n, width, height)
-    w_res = (
-        tile_transform.a
-        if abs(tile_transform.a) < abs(dst_transform.a)
-        else dst_transform.a
-    )
-    h_res = (
-        tile_transform.e
-        if abs(tile_transform.e) < abs(dst_transform.e)
-        else dst_transform.e
-    )
+    # When no output size (resolution) - Use Dataset Resolution
+    # NOTE: When we don't `fix` the output width/height, we're using the reprojected dataset resolution
+    # to calculate what is the size/transform of the VRT
+    w_res = dst_transform.a
+    h_res = dst_transform.e
+
+    # NOTE: When we have desired output height/width, we can use them to
+    # calculate the output size/transform. The VRT resolution will be aligned with the desired
+    # output resolution (if not bigger)
+    if height and width:
+        output_transform = from_bounds(w, s, e, n, width, height)
+
+        # NOTE: Here we check if the Output Resolution is higher thant the dataset resolution (OverZoom)
+        # When not overzooming we don't want to use the output Width/Height to calculate the transform
+        # See issues https://github.com/cogeotiff/rio-tiler/pull/648
+        w_res = (
+            output_transform.a
+            if abs(output_transform.a) < abs(dst_transform.a)
+            else dst_transform.a
+        )
+        h_res = (
+            output_transform.e
+            if abs(output_transform.e) < abs(dst_transform.e)
+            else dst_transform.e
+        )
 
-    # TODO: Explain
     vrt_width = max(1, round((e - w) / w_res))
     vrt_height = max(1, round((s - n) / h_res))
     vrt_transform = from_bounds(w, s, e, n, vrt_width, vrt_height)
-
     return vrt_transform, vrt_width, vrt_height
 
 
 def has_alpha_band(src_dst: Union[DatasetReader, DatasetWriter, WarpedVRT]) -> bool:
     """Check for alpha band or mask in source."""
     if (
         any(MaskFlags.alpha in flags for flags in src_dst.mask_flag_enums)
```

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/__init__.py` & `rio_tiler-6.5.0/rio_tiler/cmap_data/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/accent.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/accent.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/accent_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/accent_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/afmhot.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/afmhot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/afmhot_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/afmhot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/algae.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/algae.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/algae_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/algae_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/amp.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/amp.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/amp_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/amp_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/autumn.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/autumn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/autumn_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/autumn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/balance.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/balance.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/balance_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/balance_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/binary.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/binary.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/binary_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/binary_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/blues.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/blues.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/blues_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/blues_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/bone.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/bone.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/bone_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/bone_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/brbg.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/brbg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/brbg_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/brbg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/brg.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/brg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/brg_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/brg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/bugn.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/bugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/bugn_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/bugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/bupu.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/bupu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/bupu_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/bupu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/bwr.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/bwr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/bwr_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/bwr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/cfastie.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/cfastie.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/cividis.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/cividis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/cividis_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/cividis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/cmrmap.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/cmrmap.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/cmrmap_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/cmrmap_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/cool.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/cool.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/cool_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/cool_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/coolwarm.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/coolwarm.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/coolwarm_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/coolwarm_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/copper.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/copper.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/copper_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/copper_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/cubehelix.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/cubehelix.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/cubehelix_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/cubehelix_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/curl.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/curl.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/curl_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/curl_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/dark2.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/dark2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/dark2_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/dark2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/deep.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/deep.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/deep_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/deep_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/delta.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/delta.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/delta_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/delta_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/dense.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/dense.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/dense_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/dense_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/diff.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/diff.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/diff_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/diff_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/flag.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/flag.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/flag_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/flag_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_earth.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_earth.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_earth_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_earth_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_gray.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_gray_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_heat.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_heat.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_heat_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_heat_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_ncar.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_ncar.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_ncar_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_ncar_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_rainbow.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_rainbow_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_stern.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_stern.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_stern_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_stern_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_yarg.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_yarg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gist_yarg_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gist_yarg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gnbu.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gnbu_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gnuplot.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gnuplot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gnuplot2.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gnuplot2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gnuplot2_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gnuplot2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gnuplot_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gnuplot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gray.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/gray_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/greens.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/greens.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/greens_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/greens_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/greys.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/greys.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/greys_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/greys_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/haline.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/haline.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/haline_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/haline_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/hot.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/hot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/hot_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/hot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/hsv.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/hsv.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/hsv_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/hsv_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ice.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ice.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ice_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ice_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/inferno.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/inferno.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/inferno_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/inferno_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/jet.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/jet.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/jet_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/jet_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/magma.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/magma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/magma_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/magma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/matter.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/matter.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/matter_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/matter_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/nipy_spectral.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/nipy_spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/nipy_spectral_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/nipy_spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ocean.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ocean.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ocean_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ocean_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/oranges.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/oranges.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/oranges_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/oranges_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/orrd.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/orrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/orrd_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/orrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/oxy.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/oxy.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/oxy_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/oxy_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/paired.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/paired.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/paired_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/paired_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pastel1.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pastel1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pastel1_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pastel1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pastel2.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pastel2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pastel2_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pastel2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/phase.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/phase.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/phase_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/phase_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pink.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pink.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pink_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pink_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/piyg.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/piyg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/piyg_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/piyg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/plasma.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/plasma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/plasma_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/plasma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/prgn.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/prgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/prgn_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/prgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/prism.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/prism.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/prism_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/prism_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pubu.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pubu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pubu_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pubu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pubugn.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pubugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/pubugn_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/pubugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/puor.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/puor.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/puor_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/puor_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/purd.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/purd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/purd_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/purd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/purples.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/purples.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/purples_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/purples_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rain.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rain.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rain_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rain_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rainbow.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rainbow_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdbu.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdbu_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdgy.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdgy.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdgy_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdgy_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdpu.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdpu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdpu_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdpu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdylbu.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdylbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdylbu_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdylbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdylgn.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rdylgn_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rdylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/reds.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/reds.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/reds_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/reds_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/rplumbo.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/rplumbo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/schwarzwald.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/schwarzwald.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/seismic.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/seismic.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/seismic_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/seismic_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/set1.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/set1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/set1_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/set1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/set2.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/set2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/set2_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/set2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/set3.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/set3.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/set3_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/set3_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/solar.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/solar.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/solar_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/solar_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/spectral.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/spectral_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/speed.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/speed.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/speed_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/speed_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/spring.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/spring.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/spring_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/spring_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/summer.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/summer.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/summer_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/summer_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tab10.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tab10.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tab10_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tab10_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tab20.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tab20.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tab20_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tab20_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tab20b.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tab20b.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tab20b_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tab20b_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tab20c.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tab20c.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tab20c_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tab20c_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tarn.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tarn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tarn_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tarn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tempo.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tempo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/tempo_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/tempo_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/terrain.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/terrain.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/terrain_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/terrain_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/thermal.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/thermal.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/thermal_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/thermal_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/topo.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/topo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/topo_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/topo_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/turbid.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/turbid.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/turbid_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/turbid_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/turbo.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/turbo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/turbo_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/turbo_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/twilight.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/twilight.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/twilight_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/twilight_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/twilight_shifted.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/twilight_shifted.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/twilight_shifted_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/twilight_shifted_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/viridis.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/viridis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/viridis_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/viridis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/winter.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/winter.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/winter_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/winter_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/wistia.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/wistia.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/wistia_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/wistia_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ylgn.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ylgn_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ylgnbu.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ylgnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ylgnbu_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ylgnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ylorbr.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ylorbr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ylorbr_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ylorbr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ylorrd.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ylorrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/cmap_data/ylorrd_r.npy` & `rio_tiler-6.5.0/rio_tiler/cmap_data/ylorrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/io/base.py` & `rio_tiler-6.5.0/rio_tiler/io/base.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/io/rasterio.py` & `rio_tiler-6.5.0/rio_tiler/io/rasterio.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/io/stac.py` & `rio_tiler-6.5.0/rio_tiler/io/stac.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/io/xarray.py` & `rio_tiler-6.5.0/rio_tiler/io/xarray.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/mosaic/reader.py` & `rio_tiler-6.5.0/rio_tiler/mosaic/reader.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/mosaic/methods/__init__.py` & `rio_tiler-6.5.0/rio_tiler/mosaic/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/mosaic/methods/base.py` & `rio_tiler-6.5.0/rio_tiler/mosaic/methods/base.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/rio_tiler/mosaic/methods/defaults.py` & `rio_tiler-6.5.0/rio_tiler/mosaic/methods/defaults.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/.gitignore` & `rio_tiler-6.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/LICENSE` & `rio_tiler-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/README.md` & `rio_tiler-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/pyproject.toml` & `rio_tiler-6.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.7/PKG-INFO` & `rio_tiler-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rio-tiler
-Version: 6.4.7
+Version: 6.5.0
 Summary: User friendly Rasterio plugin to read raster datasets.
 Project-URL: Homepage, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Documentation, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Issues, https://github.com/cogeotiff/rio-tiler/issues
 Project-URL: Source, https://github.com/cogeotiff/rio-tiler
 Project-URL: Changelog, https://cogeotiff.github.io/rio-tiler/release-notes/
 Author-email: Vincent Sarago <vincent@developmentseed.com>
```

