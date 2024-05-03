# Comparing `tmp/GaiaXPy-2.1.0.tar.gz` & `tmp/gaiaxpy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaiaXPy-2.1.0.tar", last modified: Fri Aug 11 19:22:41 2023, max compression
+gzip compressed data, was "gaiaxpy-2.1.1.tar", last modified: Fri May  3 10:34:19 2024, max compression
```

## Comparing `GaiaXPy-2.1.0.tar` & `gaiaxpy-2.1.1.tar`

### file list

```diff
@@ -1,272 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.207571 GaiaXPy-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.171570 GaiaXPy-2.1.0/GaiaXPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-11 19:22:41.000000 GaiaXPy-2.1.0/GaiaXPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-08-11 19:22:41.000000 GaiaXPy-2.1.0/GaiaXPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-11 19:22:41.000000 GaiaXPy-2.1.0/GaiaXPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-11 19:22:41.000000 GaiaXPy-2.1.0/GaiaXPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-11 19:22:41.000000 GaiaXPy-2.1.0/GaiaXPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-11 19:22:41.207571 GaiaXPy-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.171570 GaiaXPy-2.1.0/gaiaxpy/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.175570 GaiaXPy-2.1.0/gaiaxpy/calibrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/calibrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/calibrator/calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/calibrator/external_instrument_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.175570 GaiaXPy-2.1.0/gaiaxpy/cholesky/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/cholesky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/cholesky/cholesky.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.175570 GaiaXPy-2.1.0/gaiaxpy/colour_equation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/colour_equation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/colour_equation/xp_filter_system_colour_equation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.175570 GaiaXPy-2.1.0/gaiaxpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)   211358 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/OptimisedCalibratedBases_BpId32_RpId37_withNormalisation.xml
--rw-r--r--   0 runner    (1001) docker     (123)    20430 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/TabulatedDispersionFunction-DR3-v375wiv142r_20200610.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/available_systems.txt
--rw-r--r--   0 runner    (1001) docker     (123)   112634 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v211w_bases.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v211w_dispersion.csv
--rw-r--r--   0 runner    (1001) docker     (123)    32220 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v211w_response.csv
--rw-r--r--   0 runner    (1001) docker     (123)    91695 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v375wi_bases.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v375wi_dispersion.csv
--rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v375wi_response.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.179571 GaiaXPy-2.1.0/gaiaxpy/config/colour_eq_files/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/colour_eq_files/JkcStd_colour_eq.ini
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/colour_eq_files/SdssStd_colour_eq.ini
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.179571 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-ElsCustomW09S2-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-EuclidVis-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Gaia2-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-GaiaDr3Vega-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HipparcosTycho-correction-factors-old.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HipparcosTycho-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HstAcswfc-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HstHugsStd-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HstWfc3uvis-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HstWfpc2-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Iphas-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Jkc-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-JkcStd-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20163 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Jpas-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Jplus-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-JwstNircam-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Panstarrs1-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Panstarrs1Std-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Pristine-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Sdss-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-SdssStd-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-SkyMapper-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Stromgren-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-StromgrenStd-correction-factors.csv
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Wfirst-correction-factors.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.187571 GaiaXPy-2.1.0/gaiaxpy/config/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Decam_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    28743 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_ElsCustomW09S2_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_EuclidVis_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    56799 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Gaia2_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_GaiaDr3Ab_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_GaiaDr3Vega_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_GaiaNominal_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)   178223 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HCustom_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HalphaCustomAb_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HalphaCustom_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HipparcosTycho_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    26283 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HstAcswfc_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HstHugsStd_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)   101196 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HstWfc3uvis_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    52172 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HstWfpc2_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    23463 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_IphasCustomW09S2_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    23460 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_IphasCustomW09_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_IphasCustom_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Iphas_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_JkcStd_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Jkc_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)   169357 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Jpas_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    34172 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Jplus_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_JwstNircam_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    21322 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Lsst_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Panstarrs1Std_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Panstarrs1_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Pristine_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    18126 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_SdssStd_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Sdss_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_SkyMapper_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    24906 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_SscAb_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_StromgrenStd_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Stromgren_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)    31671 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Ucustom_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Wfirst_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)   930529 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_v211wv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)   938664 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_v375wiv142r.xml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    92856 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/rpC03_v142r_bases.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/rpC03_v142r_dispersion.csv
--rw-r--r--   0 runner    (1001) docker     (123)    32212 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/config/rpC03_v142r_response.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.191571 GaiaXPy-2.1.0/gaiaxpy/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/converter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/converter/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.191571 GaiaXPy-2.1.0/gaiaxpy/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/custom_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/dispersion_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/generic_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/generic_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/nature.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/satellite.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/core/xml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.191571 GaiaXPy-2.1.0/gaiaxpy/error_correction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/error_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/error_correction/error_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.191571 GaiaXPy-2.1.0/gaiaxpy/file_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/file_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/file_parser/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/file_parser/parse_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/file_parser/parse_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/file_parser/parse_internal_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/file_parser/parse_internal_sampled.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/file_parser/parse_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/file_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.195571 GaiaXPy-2.1.0/gaiaxpy/generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/internal_photometric_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/multi_synthetic_photometry_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/photometric_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/regular_photometric_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/standardised_photometric_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/synthetic_photometry_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/generator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.195571 GaiaXPy-2.1.0/gaiaxpy/input_reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/input_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/input_reader/archive_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/input_reader/dataframe_numpy_array_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/input_reader/dataframe_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/input_reader/dataframe_string_array_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/input_reader/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/input_reader/input_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/input_reader/list_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/input_reader/query_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.195571 GaiaXPy-2.1.0/gaiaxpy/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/output/continuous_spectra_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.195571 GaiaXPy-2.1.0/gaiaxpy/output/ecsv_headers/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/output/ecsv_headers/headers_dict.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/output/output_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/output/photometry_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/output/sampled_spectra_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.195571 GaiaXPy-2.1.0/gaiaxpy/plotter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/plotter/multi_absolute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/plotter/multi_xp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/plotter/plot_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/plotter/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/plotter/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.199571 GaiaXPy-2.1.0/gaiaxpy/spectrum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/absolute_sampled_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/generic_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/multi_synthetic_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/sampled_basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/sampled_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/single_synthetic_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/spectral_energy_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/xp_continuous_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/xp_sampled_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/gaiaxpy/spectrum/xp_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-11 19:22:41.207571 GaiaXPy-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1953 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.199571 GaiaXPy-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.199571 GaiaXPy-2.1.0/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/files/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.199571 GaiaXPy-2.1.0/tests/test_calibrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_calibrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_calibrator/calibrator_solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_calibrator/test_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_calibrator/test_calibrator_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_calibrator/test_calibrator_missing_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_calibrator/test_calibrator_with_covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_calibrator/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_calibrator/test_external_instrument_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_calibrator/test_truncation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.199571 GaiaXPy-2.1.0/tests/test_cholesky/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_cholesky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_cholesky/cholesky_solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_cholesky/test_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_cholesky/test_cholesky_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_cholesky/test_cholesky_missing_bp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.199571 GaiaXPy-2.1.0/tests/test_colour_equation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_colour_equation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_colour_equation/colour_equation_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_colour_equation/test_xp_filter_system_colour_equation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.203571 GaiaXPy-2.1.0/tests/test_converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_converter/converter_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_converter/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_converter/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_converter/test_converter_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_converter/test_converter_missing_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_converter/test_converter_with_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.203571 GaiaXPy-2.1.0/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_core/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_core/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_core/test_dispersion_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_core/test_generic_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.203571 GaiaXPy-2.1.0/tests/test_error_correction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_error_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_error_correction/error_correction_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_error_correction/test_error_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.203571 GaiaXPy-2.1.0/tests/test_file_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_file_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_file_parser/test_parse_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_file_parser/test_parse_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_file_parser/test_parse_internal_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_file_parser/test_parse_internal_sampled.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.203571 GaiaXPy-2.1.0/tests/test_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/generator_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/test_generator_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/test_generator_missing_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/test_internal_photometric_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/test_multi_synthetic_photometry_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/test_photometric_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/test_single_synthetic_photometry_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_generator/test_synthetic_photometry_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.207571 GaiaXPy-2.1.0/tests/test_input_reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_input_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_input_reader/test_input_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_input_reader/test_input_reader_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_input_reader/test_input_reader_missing_bp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.207571 GaiaXPy-2.1.0/tests/test_output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_output/test_save_cont_raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.207571 GaiaXPy-2.1.0/tests/test_plotter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_plotter/test_multi_absolute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_plotter/test_multi_xp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_plotter/test_single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.207571 GaiaXPy-2.1.0/tests/test_spectrum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_spectrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_spectrum/test_absolute_sampled_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_spectrum/test_generic_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_spectrum/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_spectrum/test_xp_continuous_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_spectrum/test_xp_sampled_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/test_spectrum/test_xp_spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:41.207571 GaiaXPy-2.1.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-08-11 19:22:31.000000 GaiaXPy-2.1.0/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.085541 gaiaxpy-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-03 10:34:19.085541 gaiaxpy-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:34:19.085541 gaiaxpy-2.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1501 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.049540 gaiaxpy-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.085541 gaiaxpy-2.1.1/src/GaiaXPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-03 10:34:19.000000 gaiaxpy-2.1.1/src/GaiaXPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-03 10:34:19.000000 gaiaxpy-2.1.1/src/GaiaXPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:34:19.000000 gaiaxpy-2.1.1/src/GaiaXPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 10:34:19.000000 gaiaxpy-2.1.1/src/GaiaXPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 10:34:19.000000 gaiaxpy-2.1.1/src/GaiaXPy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.053540 gaiaxpy-2.1.1/src/gaiaxpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.053540 gaiaxpy-2.1.1/src/gaiaxpy/calibrator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/calibrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12117 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/calibrator/calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/calibrator/external_instrument_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.053540 gaiaxpy-2.1.1/src/gaiaxpy/cholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/cholesky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/cholesky/cholesky.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.053540 gaiaxpy-2.1.1/src/gaiaxpy/colour_equation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/colour_equation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/colour_equation/xp_filter_system_colour_equation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.057540 gaiaxpy-2.1.1/src/gaiaxpy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)   314302 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/OptimisedCalibratedBases_BpId32_RpId37_withNormalisation.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20430 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/TabulatedDispersionFunction-DR3-v375wiv142r_20200610.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/available_systems.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   112634 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v211w_bases.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v211w_dispersion.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    32220 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v211w_response.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    91695 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v375wi_bases.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v375wi_dispersion.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    32661 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v375wi_response.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.057540 gaiaxpy-2.1.1/src/gaiaxpy/config/colour_eq_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/colour_eq_files/JkcStd_colour_eq.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/colour_eq_files/SdssStd_colour_eq.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.061540 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-ElsCustomW09S2-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-EuclidVis-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Gaia2-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-GaiaDr3Vega-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HipparcosTycho-correction-factors-old.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HipparcosTycho-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HstAcswfc-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HstHugsStd-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HstWfc3uvis-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HstWfpc2-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Iphas-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Jkc-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-JkcStd-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20163 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Jpas-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Jplus-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-JwstNircam-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Panstarrs1-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Panstarrs1Std-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Pristine-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Sdss-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-SdssStd-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-SkyMapper-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Stromgren-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-StromgrenStd-correction-factors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Wfirst-correction-factors.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.073541 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)    22212 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Decam_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    40857 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_ElsCustomW09S2_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_EuclidVis_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    86865 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Gaia2_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_GaiaDr3Ab_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_GaiaDr3Vega_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_GaiaNominal_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   253169 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HCustom_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    46060 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HalphaCustomAb_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    43469 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HalphaCustom_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HipparcosTycho_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    39893 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HstAcswfc_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15639 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HstHugsStd_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   153702 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HstWfc3uvis_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    79246 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HstWfpc2_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    35577 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_IphasCustomW09S2_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    35574 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_IphasCustomW09_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    26749 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_IphasCustom_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13863 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Iphas_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22468 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_JkcStd_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Jkc_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   259263 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Jpas_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    52270 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Jplus_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_JwstNircam_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    30444 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Lsst_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22219 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Panstarrs1Std_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22205 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Panstarrs1_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Pristine_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25752 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_SdssStd_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22441 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Sdss_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36115 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_SkyMapper_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    37020 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_SscAb_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_StromgrenStd_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20291 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Stromgren_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    48273 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Ucustom_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Wfirst_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1434512 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_v211wv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1442647 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_v375wiv142r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/fluxCal_20230901_renorm_bspline.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92856 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/rpC03_v142r_bases.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/rpC03_v142r_dispersion.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    32212 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/config/rpC03_v142r_response.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.073541 gaiaxpy-2.1.1/src/gaiaxpy/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9391 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/converter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/converter/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.077540 gaiaxpy-2.1.1/src/gaiaxpy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/custom_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/dispersion_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22877 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/generic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/generic_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/input_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/nature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/satellite.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/core/xml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.077540 gaiaxpy-2.1.1/src/gaiaxpy/error_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/error_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/error_correction/error_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.077540 gaiaxpy-2.1.1/src/gaiaxpy/file_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/file_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/file_parser/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/file_parser/parse_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/file_parser/parse_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10963 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/file_parser/parse_internal_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/file_parser/parse_internal_sampled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/file_parser/parse_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/file_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.077540 gaiaxpy-2.1.1/src/gaiaxpy/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/internal_photometric_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/multi_synthetic_photometry_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/photometric_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/regular_photometric_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/standardised_photometric_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/synthetic_photometry_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/generator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.081541 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/archive_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/dataframe_numpy_array_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/dataframe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/dataframe_string_array_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/hdfs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/input_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/list_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/local_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/input_reader/required_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.081541 gaiaxpy-2.1.1/src/gaiaxpy/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/output/continuous_spectra_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.081541 gaiaxpy-2.1.1/src/gaiaxpy/output/ecsv_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/output/ecsv_headers/headers_dict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/output/output_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/output/photometry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/output/sampled_spectra_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.081541 gaiaxpy-2.1.1/src/gaiaxpy/plotter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/plotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/plotter/multi_absolute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/plotter/multi_xp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/plotter/plot_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/plotter/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/plotter/single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:19.085541 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/absolute_sampled_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/calibration_absolute_sampled_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/generic_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/multi_synthetic_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/photometric_absolute_sampled_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/sampled_basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/sampled_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/single_synthetic_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/spectral_energy_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/xp_continuous_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/xp_sampled_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-03 10:34:14.000000 gaiaxpy-2.1.1/src/gaiaxpy/spectrum/xp_spectrum.py
```

### Comparing `GaiaXPy-2.1.0/LICENCE` & `gaiaxpy-2.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/README.md` & `gaiaxpy-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/__init__.py` & `gaiaxpy-2.1.1/src/gaiaxpy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+# flake8: noqa
 from .calibrator.calibrator import calibrate
 from .cholesky.cholesky import get_chi2, get_inverse_covariance_matrix, get_inverse_square_root_covariance_matrix
 from .converter.converter import convert
 from .core.dispersion_function import pwl_to_wl, wl_to_pwl, pwl_range, wl_range
-from .core.version import __version__
 from .error_correction.error_correction import apply_error_correction
 from .generator.generator import generate
 from .generator.photometric_system import PhotometricSystem, load_additional_systems, remove_additional_systems
 from .plotter.plot_spectra import plot_spectra
+from .core.version import __version__
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/calibrator/calibrator.py` & `gaiaxpy-2.1.1/src/gaiaxpy/calibrator/calibrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 ====================================
 Module for the calibrator functionality.
 """
 
 from configparser import ConfigParser
 from os.path import join
 from pathlib import Path
+from sys import stdout
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
 from gaiaxpy.config.paths import config_path, config_ini_file
 from gaiaxpy.core.config import load_xpmerge_from_xml, load_xpsampling_from_xml
-from gaiaxpy.core.generic_functions import cast_output, get_spectra_type, validate_arguments, validate_wl_sampling, \
-    parse_band
+from gaiaxpy.core.generic_functions import cast_output, validate_wl_sampling, parse_band, format_sampled_output
 from gaiaxpy.core.generic_variables import pbar_colour, pbar_units, pbar_message
 from gaiaxpy.core.satellite import BANDS, BP_WL, RP_WL
 from gaiaxpy.input_reader.input_reader import InputReader
 from gaiaxpy.output.sampled_spectra_data import SampledSpectraData
-from gaiaxpy.spectrum.absolute_sampled_spectrum import AbsoluteSampledSpectrum
 from gaiaxpy.spectrum.sampled_basis_functions import SampledBasisFunctions
 from gaiaxpy.spectrum.utils import get_covariance_matrix
 from gaiaxpy.spectrum.xp_continuous_spectrum import XpContinuousSpectrum
 from .external_instrument_model import ExternalInstrumentModel
+from ..core.input_validator import validate_save_arguments
+from ..spectrum.calibration_absolute_sampled_spectrum import CalibrationAbsoluteSampledSpectrum
 
 __FUNCTION_KEY = 'calibrator'
 
 
 def calibrate(input_object: Union[list, Path, str], sampling: np.ndarray = None, truncation: bool = False,
               output_path: Union[Path, str] = '.', output_file: str = 'output_spectra', output_format: str = None,
-              save_file: bool = True, with_correlation: bool = False, username: str = None, password: str = None) ->\
+              save_file: bool = True, with_correlation: bool = False, username: str = None, password: str = None) -> \
         (pd.DataFrame, np.ndarray):
     """
     Calibration utility: calibrates the input internally-calibrated continuously-represented mean spectra to the
     absolute system. An absolute spectrum sampled on a user-defined or default wavelength grid is created for each set
     of BP and RP input spectra. If either band is missing, the output spectrum will only cover the range covered by the
     available data.
 
@@ -64,34 +65,35 @@
     return _calibrate(input_object, sampling, truncation, output_path, output_file, output_format, save_file,
                       with_correlation=with_correlation, username=username, password=password)
 
 
 def _calibrate(input_object: Union[list, Path, str], sampling: np.ndarray = None, truncation: bool = False,
                output_path: Union[Path, str] = '.', output_file: str = 'output_spectra', output_format: str = None,
                save_file: bool = True, with_correlation: bool = False, username: str = None, password: str = None,
-               bp_model: str = 'v375wi', rp_model: str = 'v142r', disable_info: bool = False) ->\
+               bp_model: str = 'v375wi', rp_model: str = 'v142r', disable_info: bool = False) -> \
         (pd.DataFrame, np.ndarray):
     """
-    Internal method of the calibration utility. Refer to "calibrate".
+    Internal function of the calibration utility. Refer to "calibrate".
 
     Args:
         bp_model (str): The bp model.
         rp_model (str): The rp model.
 
     Returns:
         DataFrame: A list of all sampled absolute spectra.
         ndarray: The sampling used to calibrate the spectra.
 
     Raises:
         ValueError: If the sampling is out of the expected boundaries.
     """
     validate_wl_sampling(sampling)
-    validate_arguments(_calibrate.__defaults__[3], output_file, save_file)
-    parsed_input_data, extension = InputReader(input_object, _calibrate, disable_info=disable_info, user=username,
-                                               password=password).read()
+    validate_save_arguments(_calibrate.__defaults__[3], output_file, _calibrate.__defaults__[4], output_format,
+                            save_file)
+    parsed_input_data, extension = InputReader(input_object, _calibrate, truncation=truncation,
+                                               disable_info=disable_info, user=username, password=password).read()
     xp_design_matrices, xp_merge = __generate_xp_matrices_and_merge(__FUNCTION_KEY, sampling, bp_model, rp_model)
     spectra_df, positions = __create_spectra(parsed_input_data, truncation, xp_design_matrices, xp_merge,
                                              with_correlation=with_correlation, disable_info=disable_info)
     spectra_df = cast_output(spectra_df)
     output_data = SampledSpectraData(spectra_df, positions)
     output_data.save(save_file, output_path, output_file, output_format, extension)
     return spectra_df, positions
@@ -160,16 +162,16 @@
         xp_design_matrices = load_xpsampling_from_xml(bp_model=bp_model)
         xp_design_matrices = {xp: SampledBasisFunctions.from_design_matrix(xp_sampling_grid, xp_design_matrices[xp])
                               for xp in BANDS}
     else:
         xp_merge = {xp: __create_merge(xp, sampling) for xp in BANDS}
         xp_design_matrices = {xp: SampledBasisFunctions.from_external_instrument_model(
             sampling, xp_merge[xp], ExternalInstrumentModel.from_config_csv(
-                __get_file_for_xp(xp, 'dispersion'), __get_file_for_xp(xp, 'response'), __get_file_for_xp(xp, 'bases')))
-            for xp in BANDS}
+                __get_file_for_xp(xp, 'dispersion'), __get_file_for_xp(xp, 'response'),
+                __get_file_for_xp(xp, 'bases'))) for xp in BANDS}
     return xp_design_matrices, xp_merge
 
 
 def __create_spectra(parsed_input_data: pd.DataFrame, truncation: bool, design_matrices: dict,
                      merge: dict, with_correlation: bool = False, disable_info: bool = False):
     """
      Create a DataFrame of absolute sampled spectra for each source in the parsed mean spectra file.
@@ -191,21 +193,16 @@
                  attributes 'data_type' indicating the type of spectra and 'positions' indicating the sample positions.
              positions (ndarray): 1D array of the sample positions.
      """
     parsed_spectrum_file_dict = parsed_input_data.to_dict('records')
     spectra_series = pd.Series([_create_spectrum(row, truncation, design_matrices, merge,
                                                  with_correlation=with_correlation) for row in tqdm(
         parsed_spectrum_file_dict, desc=pbar_message[__FUNCTION_KEY], unit=pbar_units[__FUNCTION_KEY], leave=False,
-        colour=pbar_colour, disable=disable_info)])
-    positions = spectra_series.iloc[0].get_positions()
-    spectra_type = get_spectra_type(spectra_series.iloc[0])
-    spectra_series = spectra_series.map(lambda x: x.spectrum_to_dict())
-    spectra_df = pd.DataFrame(spectra_series.tolist())
-    spectra_df.attrs['data_type'] = spectra_type
-    return spectra_df, positions
+        colour=pbar_colour, disable=disable_info, file=stdout)])
+    return format_sampled_output(spectra_series, with_correlation=with_correlation)
 
 
 def _create_spectrum(row, truncation, design_matrix, merge, with_correlation=False):
     """
     Create a single sampled absolute spectrum from the input continuously-represented mean spectrum and design matrix.
 
     Args:
@@ -214,16 +211,16 @@
         truncation (bool): Toggle truncation of the set of bases.
         design_matrix (ndarray): 2D array containing the basis functions sampled on the pseudo-wavelength grid (either
             user-defined or default).
         merge (dict): Dictionary containing an array of weights per BP and one for RP. These have one value per sample
             and define the contributions from BP and RP to the joined absolute spectrum.
 
     Returns:
-        AbsoluteSampledSpectrum: The absolute sampled spectrum.
+        CalibrationAbsoluteSampledSpectrum: The absolute sampled spectrum with calibration behaviour.
     """
     source_id = row['source_id']
     continuous_dict = {band: XpContinuousSpectrum(source_id, band, row[f'{band}_coefficients'],
                                                   get_covariance_matrix(row, band), row[f'{band}_standard_deviation'])
                        for band in BANDS}
     recommended_truncation = {band: row[f'{band}_n_relevant_bases'] for band in BANDS} if truncation else dict()
-    return AbsoluteSampledSpectrum(source_id, continuous_dict, design_matrix, merge, truncation=recommended_truncation,
-                                   with_correlation=with_correlation)
+    return CalibrationAbsoluteSampledSpectrum(source_id, continuous_dict, design_matrix, merge,
+                                              truncation=recommended_truncation, with_correlation=with_correlation)
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/calibrator/external_instrument_model.py` & `gaiaxpy-2.1.1/src/gaiaxpy/calibrator/external_instrument_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,19 @@
         # Dispersion
         _disp = np.genfromtxt(dispersion_path, delimiter=',')
         dispersion = dict(zip(['wavelength', 'pseudo-wavelength'], [_disp[0], _disp[1]]))
         # Response
         _resp = np.genfromtxt(response_path, delimiter=',')
         response = dict(zip(['wavelength', 'response'], [_resp[0], _resp[1]]))
         # Bases
-        bases, _ = InverseBasesParser()._parse(bases_path)
-        bases['inverseBasesCoefficients'][0] = bases['inverseBasesCoefficients'][0].reshape(
-            bases['nBases'][0], bases['nInverseBasesCoefficients'][0])
-        bases['transformationMatrix'][0] = bases['transformationMatrix'][0].reshape(
-            bases['nBases'][0], bases['nTransformedBases'][0])
+        bases, _ = InverseBasesParser().parse_file(bases_path)
+        bases = bases.iloc[0]
+        bases['inverseBasesCoefficients'] = bases['inverseBasesCoefficients'].reshape(bases['nBases'],
+                                                                                      bases['nInverseBasesCoefficients'])
+        bases['transformationMatrix'] = bases['transformationMatrix'].reshape(bases['nBases'], bases['nTransformedBases'])
         return cls(dispersion, response, bases)
 
     def get_response(self, wavelength: float) -> np.ndarray:
         """
         Get the response of the mean instrument at a certain wavelength.
 
         Args:
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/cholesky/cholesky.py` & `gaiaxpy-2.1.1/src/gaiaxpy/cholesky/cholesky.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,15 @@
     """
     output_list = [parsed_input_data['source_id']]
     for element in bands_output:
         output_list.append(element)
     return pd.DataFrame(zip(*output_list), columns=output_columns)
 
 
-def get_inverse_square_root_covariance_matrix(input_object: Union[list, Path, str],
-                                              band: Optional[Union[list, str]] = None):
+def get_inverse_square_root_covariance_matrix(input_object: Union[list, Path, str], band: Optional[str] = None):
     """
     Compute the inverse square root covariance matrix.
 
     Args:
         input_object (list/Path/str): Path to the file containing the mean spectra as downloaded from the archive in
             their continuous representation, a pandas DataFrame, a list of sources ids (string or long), or an ADQL
             query.
@@ -68,15 +67,15 @@
             for the sources in the input object if it contains more than one source or no band is passed to the
             function.
             The function will return a ndarray (of shape (55, 55)) if there is only one source ID in the input data
             and a single band is selected.
     """
     if band is not None:
         band = parse_band(band)
-    parsed_input_data, extension = InputReader(input_object, get_inverse_square_root_covariance_matrix).read()
+    parsed_input_data, extension = InputReader(input_object, get_inverse_square_root_covariance_matrix, False).read()
     if band is None:
         bands_to_process = BANDS
         output_columns = ['source_id', 'bp_inverse_square_root_covariance_matrix',
                           'rp_inverse_square_root_covariance_matrix']
     else:
         bands_to_process = [band]
         output_columns = ['source_id', f'{band}_inverse_square_root_covariance_matrix']
@@ -113,15 +112,15 @@
         # Matrix of inverse errors
         _E_inv = diag(1.0 / xp_errors)
         return dot(_L_inv, _E_inv)
     except ValueError:
         return None
 
 
-def get_inverse_covariance_matrix(input_object: Union[list, Path, str], band: str = None):
+def get_inverse_covariance_matrix(input_object: Union[list, Path, str], band: Optional[str] = None):
     """
     Compute the inverse covariance matrix.
 
     Args:
         input_object (object): Path to the file containing the mean spectra as downloaded from the archive in their
             continuous representation, a pandas DataFrame, a list of sources ids (string or long), or an ADQL query.
         band (str): Chosen band: 'bp' or 'rp'. If no band is passed, the function will compute the inverse covariance
@@ -130,15 +129,15 @@
     Returns:
         DataFrame or ndarray: DataFrame containing the source IDs and the output inverse covariance matrices for the
             sources in the input object if it contains more than one source or no band is passed to the function.
             The function will return a ndarray (of shape (55, 55)) if there is only one source ID in the input data
             and a single band is selected.
     """
     band = band if band is None else parse_band(band)
-    parsed_input_data, extension = InputReader(input_object, get_inverse_covariance_matrix).read()
+    parsed_input_data, extension = InputReader(input_object, get_inverse_covariance_matrix, False).read()
     bands_output = []
     if band is None:
         bands_to_process = BANDS
         output_columns = ['source_id', 'bp_inverse_covariance', 'rp_inverse_covariance']
     else:
         bands_to_process = [band]
         output_columns = ['source_id', f'{band}_inverse_covariance']
@@ -165,15 +164,15 @@
         _L_inv (ndarray): Inverse square root of the covariance, as computed from the function
             get_inverse_square_root_covariance_matrix.
         residuals (ndarray): Difference between the observed coefficient vector and some model prediction of it.
 
     Returns:
         float: Chi-squared value.
     """
-    if _L_inv is None or residuals is None:  # Cannot be checked with 'not' as the truth value of an array is ambiguous.
+    if _L_inv is None or residuals is None:
         raise ValueError('Input parameters cannot be None.')
     if _L_inv.shape != (55, 55):
         raise ValueError('Inverse covariance matrix shape must be (55, 55).')
     if residuals.shape != (55,):
         raise ValueError('Residuals shape must be (55,).')
     x = dot(_L_inv, residuals)
     return dot(x.T, x)
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/colour_equation/xp_filter_system_colour_equation.py` & `gaiaxpy-2.1.1/src/gaiaxpy/colour_equation/xp_filter_system_colour_equation.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 """
 
 import math
 from ast import literal_eval
 from configparser import ConfigParser
 from os import listdir
 from pathlib import Path
+from sys import stdout
 from typing import Union, Optional
 
 import numpy as np
 import pandas as pd
 from numpy import poly1d
 from tqdm import tqdm
 
 from gaiaxpy.config.paths import filters_path
-from gaiaxpy.core.generic_functions import cast_output, validate_arguments
-from gaiaxpy.core.generic_variables import pbar_colour, pbar_units
+from gaiaxpy.core.generic_functions import cast_output
+from gaiaxpy.core.generic_variables import pbar_colour, pbar_units, pbar_message
+from gaiaxpy.core.input_validator import validate_save_arguments
 from gaiaxpy.generator.photometric_system import PhotometricSystem
-from gaiaxpy.input_reader.input_reader import InputReader
+from gaiaxpy.input_reader.dataframe_reader import DataFrameReader
 from gaiaxpy.output.photometry_data import PhotometryData
 
 colour_eq_dir = Path(filters_path, '..', 'colour_eq_files')
 
 
 def __raise_key_error(key):
     """
@@ -92,20 +94,22 @@
     """
     new_system_rows = [__generate_output_row(row, system, colour_band_0, colour_band_1, systems_details) for row in
                        single_system_df.to_dict('records')]
     return pd.DataFrame(new_system_rows)
 
 
 def _generate_output_df(input_synthetic_photometry, systems_details, disable_info=False):
+    __FUNCTION_KEY = 'colour_eq'
     synth_phot_df = input_synthetic_photometry.copy()
     column_names = synth_phot_df.columns
     # Extract columns corresponding to one system
     system_keys = systems_details.keys()
-    for label in tqdm(system_keys, desc='Applying colour equation', total=len(system_keys),
-                      unit=pbar_units['colour_eq'], colour=pbar_colour, leave=False, disable=disable_info):
+    for label in tqdm(system_keys, desc=pbar_message[__FUNCTION_KEY], total=len(system_keys),
+                      unit=pbar_units[__FUNCTION_KEY], colour=pbar_colour, leave=False, disable=disable_info,
+                      file=stdout):
         filter_to_correct = systems_details[label]['filter']
         colour_band_0, colour_band_1 = _get_colour_bands(systems_details[label]['colour_index'])
         system_columns_with_colour = [column for column in column_names if column.startswith(f'{label}_') and
                                       column.endswith((f'_{filter_to_correct}', f'_{colour_band_0}',
                                                        f'_{colour_band_1}'))]
         single_system_df = synth_phot_df[system_columns_with_colour]
         corrected_system_df = __create_rows(single_system_df, label, colour_band_0, colour_band_1, systems_details)
@@ -239,17 +243,17 @@
 
 
 def _apply_colour_equation(input_synthetic_photometry: pd.DataFrame,
                            photometric_system: Union[list, PhotometricSystem] = None, output_path: str = '.',
                            output_file: str = 'corrected_photometry', output_format: Optional[str] = None,
                            save_file: bool = True, disable_info=False):
     function = apply_colour_equation
-    validate_arguments(function.__defaults__[2], output_file, save_file)
-    input_synthetic_photometry, extension = InputReader(input_synthetic_photometry, function,
-                                                        disable_info=disable_info).read()
+    validate_save_arguments(function.__defaults__[2], output_file, function.__defaults__[3], output_format, save_file)
+    input_synthetic_photometry, extension = DataFrameReader(input_synthetic_photometry, function, False,
+                                                            disable_info=disable_info).read()
     systems_to_correct = __get_systems_to_correct(photometric_system)
     systems_details = __fill_systems_details(systems_to_correct)
     output_df = _generate_output_df(input_synthetic_photometry, systems_details, disable_info=disable_info)
     output_data = PhotometryData(output_df)
     output_data.data = cast_output(output_data)
     output_data.save(save_file, output_path, output_file, output_format, extension)
     return output_data.data
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/TabulatedDispersionFunction-DR3-v375wiv142r_20200610.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/TabulatedDispersionFunction-DR3-v375wiv142r_20200610.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v211w_bases.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v211w_bases.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v211w_dispersion.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v211w_dispersion.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v211w_response.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v211w_response.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v375wi_bases.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v375wi_bases.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v375wi_dispersion.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v375wi_dispersion.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/bpC03_v375wi_response.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/bpC03_v375wi_response.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/colour_eq_files/JkcStd_colour_eq.ini` & `gaiaxpy-2.1.1/src/gaiaxpy/config/colour_eq_files/JkcStd_colour_eq.ini`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/colour_eq_files/SdssStd_colour_eq.ini` & `gaiaxpy-2.1.1/src/gaiaxpy/config/colour_eq_files/SdssStd_colour_eq.ini`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-ElsCustomW09S2-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-ElsCustomW09S2-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Gaia2-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Gaia2-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-GaiaDr3Vega-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-GaiaDr3Vega-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HipparcosTycho-correction-factors-old.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HipparcosTycho-correction-factors-old.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HipparcosTycho-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HipparcosTycho-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HstAcswfc-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HstAcswfc-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HstHugsStd-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HstHugsStd-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HstWfc3uvis-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HstWfc3uvis-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-HstWfpc2-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-HstWfpc2-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Iphas-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Iphas-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Jkc-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Jkc-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-JkcStd-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-JkcStd-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Jpas-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Jpas-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Jplus-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Jplus-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-JwstNircam-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-JwstNircam-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Panstarrs1-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Panstarrs1-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Panstarrs1Std-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Panstarrs1Std-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Pristine-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Pristine-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Sdss-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Sdss-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-SdssStd-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-SdssStd-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-SkyMapper-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-SkyMapper-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Stromgren-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Stromgren-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-StromgrenStd-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-StromgrenStd-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/correction_tables/DIDREQ-465-Wfirst-correction-factors.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/correction_tables/DIDREQ-465-Wfirst-correction-factors.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HstAcswfc_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Lsst_v375wiv142r.xml`

 * *Files 26% similar despite different names*

#### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HstAcswfc_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Lsst_v375wiv142r.xml`

```diff
@@ -1,1068 +1,720 @@
 <?xml version="1.0" encoding="utf-8"?>
 <config>
   <solutionId>4545469030156206114</solutionId>
-  <bands n="9">
-    <item>f435w</item>
-    <item>f475w</item>
-    <item>f550m</item>
-    <item>f555w</item>
-    <item>f606w</item>
-    <item>f625w</item>
-    <item>f775w</item>
-    <item>f814w</item>
-    <item>f850lp</item>
+  <bands n="6">
+    <item>u</item>
+    <item>g</item>
+    <item>r</item>
+    <item>i</item>
+    <item>z</item>
+    <item>y</item>
   </bands>
   <XpSampling>
     <bpSampledBases dimension="55">
-      <value>1.71951e-20</value>
-      <value>-4.80708e-20</value>
-      <value>3.84030e-20</value>
-      <value>-3.96887e-20</value>
-      <value>2.54947e-20</value>
-      <value>4.36764e-21</value>
-      <value>1.30227e-20</value>
-      <value>-4.60500e-21</value>
-      <value>2.55398e-21</value>
-      <value>-5.59468e-21</value>
-      <value>1.34263e-21</value>
-      <value>6.85954e-21</value>
-      <value>-5.80962e-21</value>
-      <value>1.65935e-21</value>
-      <value>-9.24924e-21</value>
-      <value>-2.36001e-21</value>
-      <value>-1.18295e-20</value>
-      <value>6.75675e-21</value>
-      <value>-1.55120e-20</value>
-      <value>1.58720e-20</value>
-      <value>-3.19268e-21</value>
-      <value>-1.86547e-20</value>
-      <value>5.91610e-21</value>
-      <value>9.83964e-21</value>
-      <value>-9.83833e-21</value>
-      <value>-3.68850e-21</value>
-      <value>-5.65641e-21</value>
-      <value>2.60691e-20</value>
-      <value>-1.68272e-20</value>
-      <value>1.67813e-20</value>
-      <value>1.07560e-21</value>
-      <value>-9.55126e-21</value>
-      <value>-7.89636e-21</value>
-      <value>1.84291e-21</value>
-      <value>1.08824e-21</value>
-      <value>1.88730e-20</value>
-      <value>2.95735e-22</value>
-      <value>1.68817e-21</value>
-      <value>1.33433e-20</value>
-      <value>2.55963e-21</value>
-      <value>-5.49471e-21</value>
-      <value>-1.61757e-21</value>
-      <value>2.14810e-20</value>
-      <value>1.09366e-20</value>
-      <value>-1.44143e-20</value>
-      <value>3.52717e-20</value>
-      <value>7.27807e-21</value>
-      <value>1.23365e-21</value>
-      <value>5.04128e-21</value>
-      <value>-3.15877e-21</value>
-      <value>-3.67120e-21</value>
-      <value>-1.65444e-21</value>
-      <value>-8.32014e-21</value>
-      <value>1.18017e-21</value>
-      <value>-7.26485e-21</value>
-      <value>2.00380e-20</value>
-      <value>-3.54937e-20</value>
-      <value>1.54193e-20</value>
-      <value>3.88010e-21</value>
-      <value>-7.98857e-21</value>
-      <value>-3.49429e-21</value>
-      <value>6.35343e-22</value>
-      <value>-1.35321e-21</value>
-      <value>4.14276e-21</value>
-      <value>-1.43015e-22</value>
-      <value>-3.91279e-22</value>
-      <value>-1.28356e-21</value>
-      <value>6.10883e-21</value>
-      <value>6.49344e-22</value>
-      <value>-6.17984e-21</value>
-      <value>-6.19987e-21</value>
-      <value>-5.95298e-21</value>
-      <value>-6.29348e-21</value>
-      <value>-1.46351e-22</value>
-      <value>-1.05432e-21</value>
-      <value>4.31997e-21</value>
-      <value>6.73044e-21</value>
-      <value>5.76307e-21</value>
-      <value>1.93782e-21</value>
-      <value>-4.37959e-21</value>
-      <value>-1.67540e-21</value>
-      <value>8.53478e-23</value>
-      <value>-2.05997e-21</value>
-      <value>6.96184e-21</value>
-      <value>-1.32343e-21</value>
-      <value>8.94720e-22</value>
-      <value>1.70456e-21</value>
-      <value>1.40153e-21</value>
-      <value>-2.21881e-21</value>
-      <value>-1.24827e-21</value>
-      <value>-2.74522e-21</value>
-      <value>1.32611e-21</value>
-      <value>-1.38323e-21</value>
-      <value>-1.37083e-21</value>
-      <value>-8.56104e-22</value>
-      <value>4.56942e-22</value>
-      <value>-9.76798e-23</value>
-      <value>-4.61284e-21</value>
-      <value>-2.72055e-21</value>
-      <value>5.80831e-21</value>
-      <value>-5.12410e-21</value>
-      <value>-2.49600e-21</value>
-      <value>1.28267e-21</value>
-      <value>5.11426e-21</value>
-      <value>1.54033e-21</value>
-      <value>5.43284e-21</value>
-      <value>1.15886e-21</value>
-      <value>-3.23513e-21</value>
-      <value>-6.60558e-22</value>
-      <value>4.00410e-22</value>
-      <value>2.47393e-20</value>
-      <value>-5.34716e-21</value>
-      <value>-2.31817e-20</value>
-      <value>2.15336e-20</value>
-      <value>3.73421e-20</value>
-      <value>1.42861e-20</value>
-      <value>2.28972e-20</value>
-      <value>-8.09251e-21</value>
-      <value>-3.93793e-21</value>
-      <value>-1.86573e-20</value>
-      <value>-5.25380e-21</value>
-      <value>-2.51356e-20</value>
-      <value>-1.16356e-20</value>
-      <value>4.78516e-22</value>
-      <value>1.93973e-21</value>
-      <value>-1.78105e-21</value>
-      <value>-9.29982e-21</value>
-      <value>-2.67448e-20</value>
-      <value>2.48525e-22</value>
-      <value>-1.17194e-20</value>
-      <value>2.88761e-20</value>
-      <value>1.57826e-20</value>
-      <value>2.44034e-20</value>
-      <value>2.06045e-21</value>
-      <value>-2.03406e-20</value>
-      <value>-1.06188e-20</value>
-      <value>-5.93812e-21</value>
-      <value>5.73263e-21</value>
-      <value>1.84891e-20</value>
-      <value>1.32781e-21</value>
-      <value>4.96695e-21</value>
-      <value>-1.38671e-21</value>
-      <value>2.87025e-21</value>
-      <value>-1.28516e-20</value>
-      <value>-3.16961e-21</value>
-      <value>-1.31702e-21</value>
-      <value>3.47810e-21</value>
-      <value>-3.63626e-21</value>
-      <value>-7.69898e-21</value>
-      <value>-1.07954e-20</value>
-      <value>2.30829e-21</value>
-      <value>-8.10221e-21</value>
-      <value>-2.20292e-20</value>
-      <value>-7.82268e-21</value>
-      <value>1.46144e-20</value>
-      <value>-1.77197e-20</value>
-      <value>-2.21013e-21</value>
-      <value>3.78177e-21</value>
-      <value>1.13332e-20</value>
-      <value>5.83761e-21</value>
-      <value>1.61144e-20</value>
-      <value>3.85976e-21</value>
-      <value>-5.45797e-21</value>
-      <value>-4.00554e-21</value>
-      <value>3.91483e-21</value>
-      <value>2.32653e-20</value>
-      <value>-1.39387e-20</value>
-      <value>-1.32595e-20</value>
-      <value>1.91133e-20</value>
-      <value>-2.05593e-21</value>
-      <value>9.60625e-21</value>
-      <value>-1.67986e-21</value>
-      <value>1.73956e-22</value>
-      <value>-1.93560e-21</value>
-      <value>6.03843e-21</value>
-      <value>4.52511e-21</value>
-      <value>3.97732e-22</value>
-      <value>-2.16576e-21</value>
-      <value>1.01698e-21</value>
-      <value>2.13186e-21</value>
-      <value>6.80935e-21</value>
-      <value>-3.33997e-21</value>
-      <value>-8.74886e-22</value>
-      <value>9.08535e-22</value>
-      <value>-4.41422e-22</value>
-      <value>-1.65292e-21</value>
-      <value>-7.54031e-23</value>
-      <value>-1.88631e-21</value>
-      <value>-2.44308e-21</value>
-      <value>1.10390e-21</value>
-      <value>-1.69339e-21</value>
-      <value>-6.72439e-22</value>
-      <value>-1.22133e-21</value>
-      <value>-3.91177e-22</value>
-      <value>1.72732e-22</value>
-      <value>7.56359e-22</value>
-      <value>-7.66390e-22</value>
-      <value>1.75305e-23</value>
-      <value>-5.01021e-22</value>
-      <value>5.66375e-22</value>
-      <value>1.06837e-21</value>
-      <value>-5.13862e-22</value>
-      <value>1.99279e-22</value>
-      <value>1.96012e-22</value>
-      <value>1.17214e-22</value>
-      <value>-2.98125e-22</value>
-      <value>-4.03989e-22</value>
-      <value>8.82960e-22</value>
-      <value>6.23137e-22</value>
-      <value>-1.87878e-21</value>
-      <value>1.61482e-21</value>
-      <value>1.25161e-21</value>
-      <value>2.70873e-22</value>
-      <value>-1.83349e-21</value>
-      <value>-3.85231e-22</value>
-      <value>-2.04280e-21</value>
-      <value>-2.29618e-22</value>
-      <value>1.35395e-21</value>
-      <value>1.23721e-23</value>
-      <value>2.22392e-22</value>
-      <value>1.56461e-20</value>
-      <value>-2.40742e-21</value>
-      <value>-8.45939e-21</value>
-      <value>1.31042e-21</value>
-      <value>-6.60010e-21</value>
-      <value>3.27517e-21</value>
-      <value>2.80977e-22</value>
-      <value>1.95337e-22</value>
-      <value>-2.58173e-21</value>
-      <value>-2.66219e-21</value>
-      <value>-1.17259e-21</value>
-      <value>-2.35677e-21</value>
-      <value>-2.20944e-21</value>
-      <value>1.31966e-21</value>
-      <value>-2.64217e-22</value>
-      <value>1.39576e-21</value>
-      <value>-2.32017e-21</value>
-      <value>-4.18918e-21</value>
-      <value>1.07269e-22</value>
-      <value>7.57091e-22</value>
-      <value>-1.04120e-21</value>
-      <value>2.61958e-23</value>
-      <value>-6.20914e-22</value>
-      <value>-1.20312e-22</value>
-      <value>-1.51003e-21</value>
-      <value>1.07913e-21</value>
-      <value>-1.23248e-21</value>
-      <value>-6.21945e-22</value>
-      <value>-1.86709e-22</value>
-      <value>-3.81903e-22</value>
-      <value>-4.86074e-22</value>
-      <value>3.18039e-22</value>
-      <value>1.17333e-22</value>
-      <value>5.93854e-23</value>
-      <value>-2.40111e-22</value>
-      <value>2.07456e-22</value>
-      <value>-4.10532e-24</value>
-      <value>5.42829e-24</value>
-      <value>9.91771e-22</value>
-      <value>5.48303e-22</value>
-      <value>-2.75232e-22</value>
-      <value>1.32709e-22</value>
-      <value>1.51332e-21</value>
-      <value>4.22424e-22</value>
-      <value>-5.50279e-22</value>
-      <value>2.03592e-21</value>
-      <value>1.39789e-22</value>
-      <value>-4.10649e-22</value>
-      <value>1.89018e-23</value>
-      <value>-6.86616e-22</value>
-      <value>-4.21743e-22</value>
-      <value>-6.34802e-23</value>
-      <value>-4.50617e-22</value>
-      <value>7.56997e-22</value>
-      <value>-9.57920e-22</value>
-      <value>1.32919e-20</value>
-      <value>5.71974e-21</value>
-      <value>-1.03126e-20</value>
-      <value>-1.20682e-20</value>
-      <value>-3.58227e-21</value>
-      <value>1.17011e-21</value>
-      <value>2.25472e-21</value>
-      <value>-2.10576e-22</value>
-      <value>-1.28443e-21</value>
-      <value>-4.08370e-21</value>
-      <value>-1.22274e-21</value>
-      <value>-6.58169e-21</value>
-      <value>-5.39695e-21</value>
-      <value>2.43359e-21</value>
-      <value>2.83891e-22</value>
-      <value>-2.43909e-21</value>
-      <value>1.03132e-22</value>
-      <value>-1.79545e-21</value>
-      <value>-2.68788e-22</value>
-      <value>-9.86707e-22</value>
-      <value>1.26576e-22</value>
-      <value>-3.69533e-22</value>
-      <value>-1.39009e-21</value>
-      <value>9.11015e-22</value>
-      <value>2.00025e-22</value>
-      <value>1.57189e-21</value>
-      <value>4.18667e-22</value>
-      <value>-6.42309e-22</value>
-      <value>-1.29988e-21</value>
-      <value>-5.20707e-22</value>
-      <value>-4.94034e-22</value>
-      <value>3.01237e-22</value>
-      <value>-3.28066e-22</value>
-      <value>6.93903e-22</value>
-      <value>-1.15065e-22</value>
-      <value>2.36069e-22</value>
-      <value>-6.84316e-23</value>
-      <value>6.26233e-23</value>
-      <value>9.54327e-22</value>
-      <value>6.91042e-22</value>
-      <value>-2.51505e-22</value>
-      <value>4.57141e-22</value>
-      <value>1.83254e-21</value>
-      <value>7.21882e-22</value>
-      <value>-1.22414e-21</value>
-      <value>1.34996e-21</value>
-      <value>6.73638e-22</value>
-      <value>-6.27720e-22</value>
-      <value>-1.29262e-21</value>
-      <value>-7.94639e-22</value>
-      <value>-1.54083e-21</value>
-      <value>-1.62682e-22</value>
-      <value>1.12157e-21</value>
-      <value>8.60983e-22</value>
-      <value>-5.27021e-22</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
+      <value>4.43004855544e-33</value>
+      <value>-1.89457565869e-32</value>
+      <value>3.21427719394e-32</value>
+      <value>-3.61475541387e-32</value>
+      <value>4.32023125650e-32</value>
+      <value>7.83404906747e-32</value>
+      <value>-2.71156190133e-32</value>
+      <value>3.33917959139e-32</value>
+      <value>-1.50368200569e-31</value>
+      <value>9.68619506550e-33</value>
+      <value>-3.75058881999e-32</value>
+      <value>1.33787558199e-32</value>
+      <value>1.24483792455e-32</value>
+      <value>1.30225049056e-32</value>
+      <value>-4.21806062469e-33</value>
+      <value>-5.22301783567e-33</value>
+      <value>2.71595216153e-32</value>
+      <value>2.46672648486e-33</value>
+      <value>-2.31972981427e-32</value>
+      <value>-6.59522634280e-33</value>
+      <value>7.94449605325e-33</value>
+      <value>-3.21792834995e-32</value>
+      <value>-3.50155855056e-32</value>
+      <value>7.62548331510e-33</value>
+      <value>2.35721221229e-32</value>
+      <value>-4.15919149733e-32</value>
+      <value>-5.10068094826e-32</value>
+      <value>1.22799385763e-31</value>
+      <value>-1.48406754048e-32</value>
+      <value>-7.45203283118e-32</value>
+      <value>-3.29108367972e-33</value>
+      <value>7.23283476911e-33</value>
+      <value>-7.27748794544e-32</value>
+      <value>2.32110052948e-32</value>
+      <value>2.28368685334e-32</value>
+      <value>1.63294435066e-32</value>
+      <value>-7.06946528940e-32</value>
+      <value>5.45256520295e-32</value>
+      <value>1.08056790630e-31</value>
+      <value>-2.84457291763e-32</value>
+      <value>-1.67769426586e-31</value>
+      <value>2.59928803858e-32</value>
+      <value>-3.91168571158e-32</value>
+      <value>7.61038788313e-32</value>
+      <value>-3.35392613767e-32</value>
+      <value>-5.47784513134e-32</value>
+      <value>-4.44859365663e-32</value>
+      <value>1.22883492548e-31</value>
+      <value>-5.04948639540e-32</value>
+      <value>2.73927200912e-32</value>
+      <value>8.24569607737e-32</value>
+      <value>1.15690187361e-32</value>
+      <value>8.51033359859e-32</value>
+      <value>-9.11753218794e-33</value>
+      <value>9.29338352209e-33</value>
+      <value>1.54611846065e-32</value>
+      <value>-2.59977305324e-32</value>
+      <value>1.04380816146e-32</value>
+      <value>4.26685662194e-33</value>
+      <value>-5.30128739397e-33</value>
+      <value>-2.00509751285e-33</value>
+      <value>1.23954295426e-33</value>
+      <value>-1.07521694923e-33</value>
+      <value>3.47021445721e-33</value>
+      <value>-9.02738091495e-34</value>
+      <value>-9.49294830123e-34</value>
+      <value>1.20019858698e-33</value>
+      <value>5.83535004504e-33</value>
+      <value>-5.34111099875e-34</value>
+      <value>-2.44332192408e-33</value>
+      <value>-9.49894527630e-34</value>
+      <value>-1.61602435581e-33</value>
+      <value>-3.78229711531e-33</value>
+      <value>1.09668549083e-34</value>
+      <value>-9.55127291936e-34</value>
+      <value>-6.21409249957e-34</value>
+      <value>4.26422637251e-33</value>
+      <value>2.21600973223e-33</value>
+      <value>4.34089433825e-34</value>
+      <value>-3.23616657686e-34</value>
+      <value>-3.15289170911e-35</value>
+      <value>-3.48370000884e-34</value>
+      <value>-2.28103494222e-33</value>
+      <value>2.78589652694e-33</value>
+      <value>-1.21428392919e-33</value>
+      <value>1.46732544886e-34</value>
+      <value>7.53911753704e-34</value>
+      <value>5.38367964245e-34</value>
+      <value>-9.95414074688e-34</value>
+      <value>-4.33731056909e-34</value>
+      <value>-1.30741274233e-33</value>
+      <value>4.89031024230e-34</value>
+      <value>-1.10502904444e-34</value>
+      <value>-1.44352243627e-34</value>
+      <value>3.08038627387e-34</value>
+      <value>-3.24843848131e-35</value>
+      <value>2.54259198370e-34</value>
+      <value>-4.04103785583e-34</value>
+      <value>-4.12214511512e-34</value>
+      <value>1.14500910340e-33</value>
+      <value>-1.46995685312e-33</value>
+      <value>-1.68581905870e-34</value>
+      <value>-4.60551217996e-35</value>
+      <value>8.45040206068e-34</value>
+      <value>-2.02064596882e-34</value>
+      <value>9.27649430797e-34</value>
+      <value>1.05675493519e-34</value>
+      <value>-9.50037824141e-34</value>
+      <value>9.36695890660e-35</value>
+      <value>-3.15508853187e-34</value>
+      <value>1.95377499418e-32</value>
+      <value>7.27904172579e-33</value>
+      <value>-1.58660144605e-32</value>
+      <value>-1.52354557024e-32</value>
+      <value>-1.89279781578e-33</value>
+      <value>2.65032821990e-33</value>
+      <value>4.23156849164e-33</value>
+      <value>-6.28003664436e-34</value>
+      <value>-1.41438599310e-33</value>
+      <value>-6.69962804511e-33</value>
+      <value>-1.42193553359e-33</value>
+      <value>-7.97801230251e-33</value>
+      <value>-8.53543095021e-33</value>
+      <value>2.38139458720e-33</value>
+      <value>2.31166451299e-33</value>
+      <value>2.22455212479e-35</value>
+      <value>2.34694573113e-33</value>
+      <value>-2.88329417649e-33</value>
+      <value>2.84514198294e-34</value>
+      <value>-6.08079165518e-34</value>
+      <value>-6.64867695278e-34</value>
+      <value>-1.06648147219e-33</value>
+      <value>-2.72638323073e-33</value>
+      <value>1.20006196961e-33</value>
+      <value>2.88155152735e-34</value>
+      <value>3.06216519919e-33</value>
+      <value>1.92791399369e-34</value>
+      <value>-9.61664219599e-34</value>
+      <value>-1.93672424272e-33</value>
+      <value>-9.18903770194e-34</value>
+      <value>-1.21559507281e-33</value>
+      <value>8.09793597837e-34</value>
+      <value>-3.04158598806e-34</value>
+      <value>1.46972355140e-33</value>
+      <value>-3.71875362770e-34</value>
+      <value>-5.20999701103e-35</value>
+      <value>-1.06542285087e-36</value>
+      <value>1.37391669945e-34</value>
+      <value>1.50019720240e-33</value>
+      <value>1.31785443440e-33</value>
+      <value>-2.58562697371e-34</value>
+      <value>9.77064672021e-34</value>
+      <value>3.03950627472e-33</value>
+      <value>9.88598566167e-34</value>
+      <value>-1.34299368294e-33</value>
+      <value>2.19804671922e-33</value>
+      <value>4.60626091126e-34</value>
+      <value>-1.09367282135e-33</value>
+      <value>-1.18742537231e-33</value>
+      <value>-1.14945143271e-33</value>
+      <value>-1.68798739002e-33</value>
+      <value>-2.47803707704e-34</value>
+      <value>6.13672811480e-34</value>
+      <value>1.35165191060e-33</value>
+      <value>-1.18037221572e-33</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
     </bpSampledBases>
     <rpSampledBases dimension="55">
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>1.99490e-25</value>
-      <value>-3.82495e-25</value>
-      <value>-3.84607e-25</value>
-      <value>-3.84382e-25</value>
-      <value>-2.76172e-25</value>
-      <value>6.74279e-25</value>
-      <value>-1.01708e-25</value>
-      <value>-4.60884e-25</value>
-      <value>4.42529e-25</value>
-      <value>-2.33551e-25</value>
-      <value>1.91290e-25</value>
-      <value>3.60321e-25</value>
-      <value>-6.73040e-25</value>
-      <value>-6.83485e-25</value>
-      <value>4.82616e-26</value>
-      <value>-2.29549e-25</value>
-      <value>4.00842e-25</value>
-      <value>6.57725e-25</value>
-      <value>7.78384e-25</value>
-      <value>-4.60687e-25</value>
-      <value>1.33411e-24</value>
-      <value>6.83539e-26</value>
-      <value>2.76143e-25</value>
-      <value>-3.05435e-25</value>
-      <value>3.05470e-25</value>
-      <value>-4.15363e-25</value>
-      <value>-5.56564e-25</value>
-      <value>-1.23933e-25</value>
-      <value>-1.91743e-24</value>
-      <value>1.02729e-24</value>
-      <value>1.52727e-24</value>
-      <value>-9.61533e-25</value>
-      <value>2.40510e-24</value>
-      <value>-2.11451e-24</value>
-      <value>7.95596e-25</value>
-      <value>-1.21355e-24</value>
-      <value>-2.44902e-25</value>
-      <value>-1.97913e-24</value>
-      <value>-7.36745e-25</value>
-      <value>7.00998e-25</value>
-      <value>-2.47064e-26</value>
-      <value>5.31143e-25</value>
-      <value>-1.05328e-24</value>
-      <value>-4.75125e-25</value>
-      <value>1.61572e-24</value>
-      <value>-9.18400e-25</value>
-      <value>3.59077e-25</value>
-      <value>-4.24726e-25</value>
-      <value>1.93303e-24</value>
-      <value>1.86205e-24</value>
-      <value>6.50811e-25</value>
-      <value>3.69332e-25</value>
-      <value>-3.32651e-25</value>
-      <value>-6.43092e-25</value>
-      <value>4.07833e-26</value>
-      <value>6.12915e-21</value>
-      <value>-9.91522e-21</value>
-      <value>-7.05238e-21</value>
-      <value>-5.21811e-22</value>
-      <value>-1.47014e-21</value>
-      <value>1.44036e-21</value>
-      <value>-1.56272e-21</value>
-      <value>-3.53767e-22</value>
-      <value>-2.26075e-21</value>
-      <value>-3.76242e-21</value>
-      <value>-9.05566e-22</value>
-      <value>-5.48219e-21</value>
-      <value>-2.40361e-21</value>
-      <value>2.07968e-21</value>
-      <value>-4.20745e-21</value>
-      <value>-2.33115e-21</value>
-      <value>9.42808e-22</value>
-      <value>1.13917e-21</value>
-      <value>-5.88079e-22</value>
-      <value>-6.46940e-22</value>
-      <value>1.24156e-21</value>
-      <value>-2.39767e-21</value>
-      <value>-1.92529e-21</value>
-      <value>-2.67276e-21</value>
-      <value>-3.71881e-22</value>
-      <value>2.93286e-21</value>
-      <value>5.95216e-21</value>
-      <value>2.23824e-21</value>
-      <value>-2.37025e-21</value>
-      <value>2.51116e-21</value>
-      <value>4.41838e-21</value>
-      <value>-4.24657e-21</value>
-      <value>-7.40610e-22</value>
-      <value>2.21162e-21</value>
-      <value>-3.48136e-21</value>
-      <value>-3.38264e-22</value>
-      <value>8.74244e-22</value>
-      <value>1.24222e-21</value>
-      <value>2.88320e-22</value>
-      <value>-3.89500e-23</value>
-      <value>2.03926e-22</value>
-      <value>-2.44408e-22</value>
-      <value>-1.19000e-21</value>
-      <value>-4.46535e-22</value>
-      <value>2.63820e-21</value>
-      <value>-3.93854e-21</value>
-      <value>2.16159e-21</value>
-      <value>5.75427e-21</value>
-      <value>6.01178e-21</value>
-      <value>6.33826e-21</value>
-      <value>-5.39641e-21</value>
-      <value>-2.58853e-21</value>
-      <value>-2.41513e-23</value>
-      <value>1.10077e-21</value>
-      <value>-1.03118e-21</value>
-      <value>8.42832e-21</value>
-      <value>-1.39767e-20</value>
-      <value>-1.05236e-20</value>
-      <value>-1.10270e-21</value>
-      <value>-3.45409e-21</value>
-      <value>2.71170e-21</value>
-      <value>-2.56720e-21</value>
-      <value>-9.57104e-22</value>
-      <value>-4.39801e-21</value>
-      <value>-7.56206e-21</value>
-      <value>-1.06447e-21</value>
-      <value>-9.84223e-21</value>
-      <value>-3.18403e-21</value>
-      <value>3.90306e-21</value>
-      <value>-4.25013e-21</value>
-      <value>1.83810e-21</value>
-      <value>1.78169e-21</value>
-      <value>8.73817e-22</value>
-      <value>1.27896e-22</value>
-      <value>8.90138e-22</value>
-      <value>3.17334e-21</value>
-      <value>1.52321e-21</value>
-      <value>1.80294e-21</value>
-      <value>-6.12038e-22</value>
-      <value>-7.84963e-22</value>
-      <value>-2.29619e-21</value>
-      <value>6.51224e-21</value>
-      <value>8.18329e-21</value>
-      <value>-4.05399e-21</value>
-      <value>1.15164e-21</value>
-      <value>3.08201e-21</value>
-      <value>-3.67996e-21</value>
-      <value>4.40107e-21</value>
-      <value>-2.74616e-21</value>
-      <value>-4.69967e-21</value>
-      <value>-5.76860e-21</value>
-      <value>4.88489e-21</value>
-      <value>7.96347e-22</value>
-      <value>-2.50966e-21</value>
-      <value>3.01572e-21</value>
-      <value>-1.27308e-21</value>
-      <value>3.55338e-21</value>
-      <value>4.49715e-21</value>
-      <value>4.43978e-22</value>
-      <value>4.30253e-23</value>
-      <value>5.42515e-22</value>
-      <value>-1.31503e-21</value>
-      <value>-3.44335e-21</value>
-      <value>1.65749e-21</value>
-      <value>2.81701e-21</value>
-      <value>6.30562e-21</value>
-      <value>2.03160e-21</value>
-      <value>-5.30910e-22</value>
-      <value>-3.15366e-21</value>
-      <value>3.60460e-22</value>
-      <value>1.70130e-20</value>
-      <value>-4.10697e-21</value>
-      <value>1.10597e-20</value>
-      <value>-2.73363e-21</value>
-      <value>6.34630e-21</value>
-      <value>-3.37031e-21</value>
-      <value>3.10835e-21</value>
-      <value>5.26254e-22</value>
-      <value>8.93012e-22</value>
-      <value>6.91986e-22</value>
-      <value>-3.30290e-22</value>
-      <value>6.74611e-21</value>
-      <value>-1.92133e-21</value>
-      <value>8.85029e-22</value>
-      <value>6.92613e-22</value>
-      <value>-2.75639e-21</value>
-      <value>-4.11182e-21</value>
-      <value>7.75084e-22</value>
-      <value>-1.32657e-22</value>
-      <value>-5.93840e-23</value>
-      <value>8.62345e-22</value>
-      <value>-1.32019e-21</value>
-      <value>4.06199e-22</value>
-      <value>2.99414e-21</value>
-      <value>-1.80456e-21</value>
-      <value>1.82194e-21</value>
-      <value>2.22316e-22</value>
-      <value>-6.11329e-22</value>
-      <value>-8.96764e-22</value>
-      <value>-2.25751e-21</value>
-      <value>3.58754e-22</value>
-      <value>1.43006e-21</value>
-      <value>2.44039e-21</value>
-      <value>1.04546e-22</value>
-      <value>-1.98314e-21</value>
-      <value>2.01057e-21</value>
-      <value>2.47300e-21</value>
-      <value>-2.93577e-21</value>
-      <value>1.57847e-21</value>
-      <value>1.71336e-21</value>
-      <value>1.21953e-21</value>
-      <value>6.80168e-22</value>
-      <value>3.09373e-22</value>
-      <value>1.60578e-21</value>
-      <value>1.55463e-21</value>
-      <value>-2.18909e-21</value>
-      <value>-1.87670e-21</value>
-      <value>-5.97512e-21</value>
-      <value>1.54186e-21</value>
-      <value>-1.31595e-21</value>
-      <value>-4.26214e-22</value>
-      <value>-2.14451e-21</value>
-      <value>-8.25226e-21</value>
-      <value>-3.01348e-21</value>
-      <value>3.51444e-21</value>
-      <value>1.68794e-20</value>
-      <value>4.10819e-21</value>
-      <value>4.10690e-21</value>
-      <value>-1.02345e-22</value>
-      <value>1.76554e-21</value>
-      <value>-1.03786e-21</value>
-      <value>1.38184e-21</value>
-      <value>1.01908e-21</value>
-      <value>5.37310e-21</value>
-      <value>2.31577e-21</value>
-      <value>-3.78979e-21</value>
-      <value>2.26176e-21</value>
-      <value>9.53510e-22</value>
-      <value>-8.59912e-23</value>
-      <value>-8.50479e-22</value>
-      <value>5.72619e-22</value>
-      <value>-4.60191e-22</value>
-      <value>-8.99484e-22</value>
-      <value>-1.11897e-21</value>
-      <value>1.65437e-22</value>
-      <value>8.85194e-22</value>
-      <value>-1.68509e-22</value>
-      <value>1.89089e-21</value>
-      <value>-1.49251e-21</value>
-      <value>1.18207e-21</value>
-      <value>-6.70133e-22</value>
-      <value>-1.97807e-22</value>
-      <value>-5.71317e-22</value>
-      <value>1.81645e-21</value>
-      <value>-1.58766e-22</value>
-      <value>2.31689e-21</value>
-      <value>2.61879e-21</value>
-      <value>1.57877e-21</value>
-      <value>-3.07138e-22</value>
-      <value>-2.50102e-21</value>
-      <value>1.72716e-21</value>
-      <value>-2.47845e-22</value>
-      <value>-2.22624e-22</value>
-      <value>-6.14577e-22</value>
-      <value>-1.94290e-21</value>
-      <value>-8.62025e-22</value>
-      <value>-6.81085e-22</value>
-      <value>3.18246e-22</value>
-      <value>-4.73854e-21</value>
-      <value>8.82541e-22</value>
-      <value>-2.35874e-21</value>
-      <value>4.91515e-21</value>
-      <value>-1.83049e-21</value>
-      <value>-7.46192e-23</value>
-      <value>-6.23643e-22</value>
-      <value>2.56328e-21</value>
-      <value>6.37164e-21</value>
-      <value>-5.33680e-21</value>
-      <value>-1.04284e-21</value>
-      <value>2.97008e-21</value>
-      <value>1.62457e-20</value>
-      <value>2.20448e-20</value>
-      <value>-1.98006e-20</value>
-      <value>9.39683e-21</value>
-      <value>4.13089e-21</value>
-      <value>5.75503e-21</value>
-      <value>1.08815e-20</value>
-      <value>-9.67201e-21</value>
-      <value>-1.61315e-20</value>
-      <value>6.60222e-21</value>
-      <value>1.23248e-20</value>
-      <value>8.01331e-21</value>
-      <value>-8.72671e-21</value>
-      <value>9.67860e-21</value>
-      <value>-3.33450e-21</value>
-      <value>-3.49041e-21</value>
-      <value>-2.32073e-21</value>
-      <value>-1.60850e-20</value>
-      <value>-1.20587e-20</value>
-      <value>5.57062e-21</value>
-      <value>1.50616e-20</value>
-      <value>-5.67310e-21</value>
-      <value>1.51409e-20</value>
-      <value>-1.82955e-20</value>
-      <value>4.80260e-21</value>
-      <value>-8.30237e-21</value>
-      <value>4.95204e-21</value>
-      <value>-1.17364e-20</value>
-      <value>-1.21591e-21</value>
-      <value>-1.09098e-20</value>
-      <value>-5.87478e-21</value>
-      <value>-1.06764e-20</value>
-      <value>1.48916e-21</value>
-      <value>1.63807e-20</value>
-      <value>2.31832e-20</value>
-      <value>-8.26394e-21</value>
-      <value>3.70903e-20</value>
-      <value>-3.47000e-20</value>
-      <value>1.98642e-20</value>
-      <value>-3.65877e-20</value>
-      <value>-3.77538e-20</value>
-      <value>-7.23556e-21</value>
-      <value>1.00412e-20</value>
-      <value>-7.60490e-20</value>
-      <value>2.69138e-20</value>
-      <value>-4.25877e-20</value>
-      <value>-1.18180e-19</value>
-      <value>-5.18227e-20</value>
-      <value>1.11862e-20</value>
-      <value>-2.69289e-20</value>
-      <value>-3.34970e-20</value>
-      <value>8.37501e-21</value>
-      <value>1.34903e-19</value>
-      <value>2.70820e-20</value>
-      <value>9.35562e-20</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>9.23975562746e-33</value>
+      <value>-1.59276535715e-32</value>
+      <value>-1.22060517450e-32</value>
+      <value>-1.71573716620e-33</value>
+      <value>-1.45259065411e-33</value>
+      <value>7.97827472225e-33</value>
+      <value>-8.04331098190e-34</value>
+      <value>5.70664025349e-33</value>
+      <value>-6.12334656067e-33</value>
+      <value>-4.01850920653e-33</value>
+      <value>-2.51550978412e-33</value>
+      <value>-1.18753501192e-32</value>
+      <value>-1.39994695578e-33</value>
+      <value>5.39041321497e-33</value>
+      <value>5.05871956060e-34</value>
+      <value>3.29982323378e-33</value>
+      <value>2.69847032396e-33</value>
+      <value>7.62618358848e-34</value>
+      <value>2.62044960615e-33</value>
+      <value>5.59934149676e-35</value>
+      <value>6.42434664716e-33</value>
+      <value>1.49506488381e-34</value>
+      <value>3.29917779186e-33</value>
+      <value>-6.35377845086e-34</value>
+      <value>3.88600156298e-33</value>
+      <value>2.58279919792e-33</value>
+      <value>8.03617606207e-33</value>
+      <value>8.44052534368e-33</value>
+      <value>-4.89775402507e-33</value>
+      <value>2.39714981374e-33</value>
+      <value>5.41053402489e-33</value>
+      <value>-4.16986449179e-33</value>
+      <value>2.98761911364e-33</value>
+      <value>-2.40622252415e-33</value>
+      <value>-4.78393195989e-33</value>
+      <value>-6.14102523695e-33</value>
+      <value>3.95179146258e-33</value>
+      <value>-3.05834093527e-34</value>
+      <value>-2.98452720653e-33</value>
+      <value>3.50192829477e-33</value>
+      <value>-1.14248588382e-33</value>
+      <value>3.70058431575e-33</value>
+      <value>4.07823449887e-33</value>
+      <value>-2.41750743420e-34</value>
+      <value>1.67711557232e-33</value>
+      <value>-2.18361499244e-33</value>
+      <value>2.69355176404e-34</value>
+      <value>2.34634905675e-34</value>
+      <value>-8.53056272356e-34</value>
+      <value>1.46158046939e-33</value>
+      <value>1.87722803638e-33</value>
+      <value>3.31264327416e-34</value>
+      <value>-6.80606643573e-34</value>
+      <value>-5.41504014509e-34</value>
+      <value>6.56719614443e-34</value>
+      <value>3.23355784375e-32</value>
+      <value>-1.51866694311e-32</value>
+      <value>1.77340814295e-32</value>
+      <value>-1.19579675823e-33</value>
+      <value>6.61298139253e-33</value>
+      <value>-1.72950779312e-32</value>
+      <value>1.29529238956e-32</value>
+      <value>-9.94488573998e-33</value>
+      <value>1.48265947202e-32</value>
+      <value>7.88419325912e-33</value>
+      <value>7.28445473713e-33</value>
+      <value>-3.71666036031e-34</value>
+      <value>-1.59194568065e-33</value>
+      <value>-5.20756587323e-34</value>
+      <value>-1.04607300728e-33</value>
+      <value>-2.65278224829e-33</value>
+      <value>4.84825658026e-34</value>
+      <value>3.61305555375e-33</value>
+      <value>-4.95238440994e-33</value>
+      <value>-4.69757543681e-33</value>
+      <value>-1.45990386791e-33</value>
+      <value>-7.15683421136e-33</value>
+      <value>4.85447486418e-35</value>
+      <value>6.90885437337e-33</value>
+      <value>-2.75999557186e-33</value>
+      <value>-3.16017688519e-33</value>
+      <value>3.18095360933e-33</value>
+      <value>-5.65368575049e-33</value>
+      <value>1.67882950616e-33</value>
+      <value>9.16664131566e-34</value>
+      <value>3.20573225221e-33</value>
+      <value>-1.94788103097e-33</value>
+      <value>-2.87873745908e-33</value>
+      <value>2.85425236509e-33</value>
+      <value>1.03668644192e-33</value>
+      <value>4.59786707146e-33</value>
+      <value>-1.90915734227e-33</value>
+      <value>-7.23841116452e-33</value>
+      <value>-2.53572610765e-33</value>
+      <value>5.81426311138e-33</value>
+      <value>-1.41516374249e-33</value>
+      <value>4.20009641776e-33</value>
+      <value>5.68004770786e-33</value>
+      <value>5.16296437488e-33</value>
+      <value>-2.90186079593e-33</value>
+      <value>1.48251048375e-33</value>
+      <value>-6.12258146107e-33</value>
+      <value>1.13594069108e-32</value>
+      <value>1.33994576510e-32</value>
+      <value>1.12706685825e-32</value>
+      <value>1.60318508895e-32</value>
+      <value>5.01787140581e-33</value>
+      <value>6.98608110846e-33</value>
+      <value>-7.29212408113e-33</value>
+      <value>-7.96722846021e-33</value>
+      <value>4.19295108884e-32</value>
+      <value>4.14705856896e-32</value>
+      <value>-7.66266988119e-33</value>
+      <value>1.28783795679e-32</value>
+      <value>-3.39335548426e-32</value>
+      <value>1.02351459790e-32</value>
+      <value>-2.05973409448e-32</value>
+      <value>3.64362650473e-32</value>
+      <value>-2.71323083826e-33</value>
+      <value>-6.70003184666e-33</value>
+      <value>8.66886480085e-33</value>
+      <value>1.64974236393e-32</value>
+      <value>-1.50130167887e-32</value>
+      <value>5.11447755697e-33</value>
+      <value>-8.91117236209e-33</value>
+      <value>-1.13742925120e-33</value>
+      <value>5.10130323394e-33</value>
+      <value>-7.69978907665e-33</value>
+      <value>3.80342828431e-33</value>
+      <value>-3.40557013867e-33</value>
+      <value>-6.86270186612e-33</value>
+      <value>8.25947608012e-33</value>
+      <value>-1.01981995442e-32</value>
+      <value>5.20466865073e-33</value>
+      <value>1.44903361857e-33</value>
+      <value>2.69170528172e-33</value>
+      <value>3.71006326066e-33</value>
+      <value>-2.70603512896e-33</value>
+      <value>-9.94152229988e-33</value>
+      <value>-5.89786005958e-33</value>
+      <value>-6.17839191008e-33</value>
+      <value>-1.60708917776e-33</value>
+      <value>9.00061918048e-33</value>
+      <value>6.55410914672e-33</value>
+      <value>-3.98475078189e-33</value>
+      <value>1.48289869064e-34</value>
+      <value>-9.88738309643e-33</value>
+      <value>5.58594376938e-33</value>
+      <value>-9.48229690932e-33</value>
+      <value>-8.67539768890e-33</value>
+      <value>-4.87127414089e-33</value>
+      <value>-2.92182508767e-33</value>
+      <value>2.81099587458e-33</value>
+      <value>-1.46920700344e-32</value>
+      <value>-2.80641344299e-33</value>
+      <value>7.13901825155e-34</value>
+      <value>1.07044389313e-32</value>
+      <value>6.50072264552e-33</value>
+      <value>7.30761133830e-34</value>
+      <value>2.39657885403e-35</value>
+      <value>3.55972961236e-33</value>
+      <value>1.86233954435e-32</value>
+      <value>2.45782974269e-33</value>
+      <value>4.84505173512e-33</value>
+      <value>2.13431111426e-33</value>
+      <value>4.99962629249e-32</value>
+      <value>1.04475116299e-31</value>
+      <value>-1.75184926870e-31</value>
+      <value>4.32588439510e-32</value>
+      <value>1.22075087625e-31</value>
+      <value>9.91372942343e-33</value>
+      <value>1.86068296340e-31</value>
+      <value>-1.64785852303e-31</value>
+      <value>-2.25664263379e-31</value>
+      <value>7.29307996527e-32</value>
+      <value>1.77804203033e-31</value>
+      <value>6.58021643706e-32</value>
+      <value>-8.77852855166e-32</value>
+      <value>7.43388159080e-32</value>
+      <value>-1.39985377477e-32</value>
+      <value>-4.47080907619e-32</value>
+      <value>-3.47931348664e-32</value>
+      <value>-1.60372682475e-31</value>
+      <value>-6.08184321240e-32</value>
+      <value>6.54496630835e-32</value>
+      <value>1.39225447920e-31</value>
+      <value>-7.61593313855e-32</value>
+      <value>1.78335549211e-31</value>
+      <value>-1.90174590989e-31</value>
+      <value>3.94661384313e-32</value>
+      <value>-8.40064220260e-32</value>
+      <value>2.32829380342e-32</value>
+      <value>-9.00627385438e-32</value>
+      <value>1.36207169058e-32</value>
+      <value>-9.29633775351e-32</value>
+      <value>-3.87402098832e-32</value>
+      <value>-9.55012145096e-32</value>
+      <value>1.22447907063e-32</value>
+      <value>1.98013456758e-31</value>
+      <value>2.55562973820e-31</value>
+      <value>-1.26140728960e-31</value>
+      <value>3.25774000566e-31</value>
+      <value>-3.11138200594e-31</value>
+      <value>2.84920300253e-31</value>
+      <value>-2.82272516975e-31</value>
+      <value>-3.27805632755e-31</value>
+      <value>-9.09122474020e-32</value>
+      <value>8.51759509792e-32</value>
+      <value>-7.47941520538e-31</value>
+      <value>1.66830528328e-31</value>
+      <value>-2.61609082116e-31</value>
+      <value>-9.57235809248e-31</value>
+      <value>-2.64100862144e-31</value>
+      <value>9.19484810758e-32</value>
+      <value>-2.73136959897e-31</value>
+      <value>-1.86283909705e-31</value>
+      <value>-1.74051525557e-31</value>
+      <value>1.05687639268e-30</value>
+      <value>2.51133789234e-31</value>
+      <value>6.90400377925e-31</value>
     </rpSampledBases>
   </XpSampling>
   <XpMerge>
     <sampleMeanWavelengths>
-      <value>433.939</value>
-      <value>476.481</value>
-      <value>558.367</value>
-      <value>537.315</value>
-      <value>596.050</value>
-      <value>632.561</value>
-      <value>770.559</value>
-      <value>807.251</value>
-      <value>904.918</value>
+      <value>367.986</value>
+      <value>480.000</value>
+      <value>623.144</value>
+      <value>754.222</value>
+      <value>869.103</value>
+      <value>973.849</value>
     </sampleMeanWavelengths>
     <bpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
-      <value>1.00000</value>
-      <value>1.00000</value>
     </bpWeights>
     <rpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
-      <value>1.00000</value>
-      <value>1.00000</value>
     </rpWeights>
   </XpMerge>
   <fluxBias>
     <value>0.00000</value>
     <value>0.00000</value>
     <value>0.00000</value>
     <value>0.00000</value>
     <value>0.00000</value>
     <value>0.00000</value>
-    <value>0.00000</value>
-    <value>0.00000</value>
-    <value>0.00000</value>
   </fluxBias>
   <zeropoints>
-    <value>-25.4740</value>
-    <value>-25.6790</value>
-    <value>-26.1492</value>
-    <value>-26.0328</value>
-    <value>-26.3414</value>
-    <value>-26.5554</value>
-    <value>-27.2097</value>
-    <value>-27.3405</value>
-    <value>-27.6948</value>
+    <value>-56.1000</value>
+    <value>-56.1000</value>
+    <value>-56.1000</value>
+    <value>-56.1000</value>
+    <value>-56.1000</value>
+    <value>-56.1000</value>
   </zeropoints>
 </config>
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HstHugsStd_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_JwstNircam_v375wiv142r.xml`

 * *Files 24% similar despite different names*

#### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_HstHugsStd_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_JwstNircam_v375wiv142r.xml`

```diff
@@ -1,127 +1,71 @@
 <?xml version="1.0" encoding="utf-8"?>
 <config>
   <solutionId>4545469030156206114</solutionId>
-  <bands n="3">
-    <item>f438w</item>
-    <item>f606w</item>
-    <item>f814w</item>
+  <bands n="2">
+    <item>F070W</item>
+    <item>F090W</item>
   </bands>
   <XpSampling>
     <bpSampledBases dimension="55">
-      <value>1.73405379282e-20</value>
-      <value>-5.03005894131e-20</value>
-      <value>4.32441726302e-20</value>
-      <value>-4.15315997684e-20</value>
-      <value>1.32948554376e-20</value>
-      <value>-2.05062521110e-21</value>
-      <value>1.80740491557e-20</value>
-      <value>-1.23446545543e-20</value>
-      <value>2.78459627808e-20</value>
-      <value>5.11615402949e-22</value>
-      <value>-3.21634846834e-21</value>
-      <value>-1.27713544914e-20</value>
-      <value>1.90215898652e-20</value>
-      <value>-3.77717187430e-21</value>
-      <value>1.28351024789e-20</value>
-      <value>-4.00098945753e-21</value>
-      <value>1.15594791177e-20</value>
-      <value>-1.38443266192e-21</value>
-      <value>2.53464562022e-21</value>
-      <value>-1.13324227334e-20</value>
-      <value>1.60344760398e-21</value>
-      <value>2.21932682738e-20</value>
-      <value>-2.56458853876e-20</value>
-      <value>-6.25215545708e-21</value>
-      <value>3.53565778527e-22</value>
-      <value>2.06938062924e-21</value>
-      <value>2.03485337410e-20</value>
-      <value>-6.46041481380e-21</value>
-      <value>1.26348840177e-20</value>
-      <value>-1.14258783837e-20</value>
-      <value>1.96212972500e-20</value>
-      <value>1.49021255988e-20</value>
-      <value>-1.06608595027e-20</value>
-      <value>-1.95186176176e-20</value>
-      <value>-5.05994215323e-21</value>
-      <value>-4.46514456654e-21</value>
-      <value>-4.49281780743e-21</value>
-      <value>-1.02319052725e-21</value>
-      <value>-6.90018094570e-21</value>
-      <value>-1.76528856266e-20</value>
-      <value>3.68168766816e-21</value>
-      <value>-1.42978587748e-20</value>
-      <value>-6.64564639535e-21</value>
-      <value>1.28772094907e-20</value>
-      <value>-3.12606896393e-20</value>
-      <value>-4.46427799075e-21</value>
-      <value>3.14004111230e-20</value>
-      <value>-2.45128743129e-20</value>
-      <value>-4.25339113283e-20</value>
-      <value>-2.00361950629e-20</value>
-      <value>-1.62426252814e-20</value>
-      <value>-5.39297300927e-21</value>
-      <value>4.93409607225e-21</value>
-      <value>-4.96950257469e-22</value>
-      <value>-7.29678798113e-21</value>
-      <value>1.56461095895e-20</value>
-      <value>-2.40740786883e-21</value>
-      <value>-8.45939460024e-21</value>
-      <value>1.31042449376e-21</value>
-      <value>-6.60012058354e-21</value>
-      <value>3.27520751322e-21</value>
-      <value>2.80965716553e-22</value>
-      <value>1.95346411463e-22</value>
-      <value>-2.58173075387e-21</value>
-      <value>-2.66217626540e-21</value>
-      <value>-1.17258856019e-21</value>
-      <value>-2.35678931878e-21</value>
-      <value>-2.20947266712e-21</value>
-      <value>1.31963293768e-21</value>
-      <value>-2.64220276924e-22</value>
-      <value>1.39576397946e-21</value>
-      <value>-2.32018610904e-21</value>
-      <value>-4.18920476690e-21</value>
-      <value>1.07290066921e-22</value>
-      <value>7.57104046479e-22</value>
-      <value>-1.04121603466e-21</value>
-      <value>2.61957071545e-23</value>
-      <value>-6.20834237001e-22</value>
-      <value>-1.20298108941e-22</value>
-      <value>-1.50999970256e-21</value>
-      <value>1.07902842254e-21</value>
-      <value>-1.23247373417e-21</value>
-      <value>-6.21938254951e-22</value>
-      <value>-1.86765494805e-22</value>
-      <value>-3.81930178317e-22</value>
-      <value>-4.86117174262e-22</value>
-      <value>3.18034268109e-22</value>
-      <value>1.17313224638e-22</value>
-      <value>5.94045839322e-23</value>
-      <value>-2.40084258994e-22</value>
-      <value>2.07423478916e-22</value>
-      <value>-4.03453795767e-24</value>
-      <value>5.42020718494e-24</value>
-      <value>9.91688211976e-22</value>
-      <value>5.48266232787e-22</value>
-      <value>-2.75187939642e-22</value>
-      <value>1.32765720374e-22</value>
-      <value>1.51319145239e-21</value>
-      <value>4.22334762018e-22</value>
-      <value>-5.50154575819e-22</value>
-      <value>2.03548120144e-21</value>
-      <value>1.39725598103e-22</value>
-      <value>-4.10676783775e-22</value>
-      <value>1.87973269743e-23</value>
-      <value>-6.86567035647e-22</value>
-      <value>-4.21760201831e-22</value>
-      <value>-6.34666177389e-23</value>
-      <value>-4.50442717767e-22</value>
-      <value>7.56988193809e-22</value>
-      <value>-9.57805791592e-22</value>
+      <value>2.71339278595e-21</value>
+      <value>2.39734022562e-21</value>
+      <value>4.21349827995e-22</value>
+      <value>-2.97543385340e-21</value>
+      <value>-5.09661425818e-21</value>
+      <value>-7.09824463813e-22</value>
+      <value>2.01495376924e-21</value>
+      <value>1.21352012120e-22</value>
+      <value>-2.16533753931e-21</value>
+      <value>-6.53277409040e-21</value>
+      <value>-2.01546706683e-21</value>
+      <value>-4.07942558934e-21</value>
+      <value>-1.57565438644e-21</value>
+      <value>1.55821002259e-21</value>
+      <value>-1.31750218946e-21</value>
+      <value>-8.81261500390e-22</value>
+      <value>5.11314380319e-24</value>
+      <value>-4.12891890324e-21</value>
+      <value>-7.20530366373e-22</value>
+      <value>8.96192511856e-22</value>
+      <value>5.82250560619e-22</value>
+      <value>1.24122046989e-22</value>
+      <value>-3.06711650057e-22</value>
+      <value>1.00327695617e-21</value>
+      <value>-1.21600066111e-21</value>
+      <value>2.57427639966e-21</value>
+      <value>-4.59655845224e-22</value>
+      <value>-1.12594474255e-22</value>
+      <value>-5.14184536136e-22</value>
+      <value>-7.17505992800e-22</value>
+      <value>-1.18767061059e-21</value>
+      <value>7.55825248953e-22</value>
+      <value>-7.88562111249e-24</value>
+      <value>5.10560442995e-22</value>
+      <value>-5.91127541647e-22</value>
+      <value>-4.44688892441e-22</value>
+      <value>2.33820552414e-22</value>
+      <value>-2.05467558337e-23</value>
+      <value>9.03919424915e-22</value>
+      <value>5.66406608981e-22</value>
+      <value>-4.37519550658e-23</value>
+      <value>5.98071741681e-22</value>
+      <value>1.19182340889e-21</value>
+      <value>2.53425389243e-22</value>
+      <value>1.41600256140e-22</value>
+      <value>8.61815077105e-22</value>
+      <value>-1.20241311030e-22</value>
+      <value>-7.11054304722e-22</value>
+      <value>4.05994267947e-22</value>
+      <value>-6.63349118850e-22</value>
+      <value>1.07185066977e-22</value>
+      <value>2.11038529462e-23</value>
+      <value>-6.94092279999e-22</value>
+      <value>9.30810456808e-22</value>
+      <value>-1.09998372179e-21</value>
       <value>0.00000000000</value>
       <value>0.00000000000</value>
       <value>0.00000000000</value>
       <value>0.00000000000</value>
       <value>0.00000000000</value>
       <value>0.00000000000</value>
       <value>0.00000000000</value>
@@ -171,202 +115,142 @@
       <value>0.00000000000</value>
       <value>0.00000000000</value>
       <value>0.00000000000</value>
       <value>0.00000000000</value>
       <value>0.00000000000</value>
     </bpSampledBases>
     <rpSampledBases dimension="55">
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>6.12915075748e-21</value>
-      <value>-9.91522609178e-21</value>
-      <value>-7.05238010589e-21</value>
-      <value>-5.21809866006e-22</value>
-      <value>-1.47014345896e-21</value>
-      <value>1.44036111512e-21</value>
-      <value>-1.56272562608e-21</value>
-      <value>-3.53766213124e-22</value>
-      <value>-2.26074526137e-21</value>
-      <value>-3.76242203878e-21</value>
-      <value>-9.05567062918e-22</value>
-      <value>-5.48218960556e-21</value>
-      <value>-2.40360814662e-21</value>
-      <value>2.07967933285e-21</value>
-      <value>-4.20744592588e-21</value>
-      <value>-2.33115271595e-21</value>
-      <value>9.42809601177e-22</value>
-      <value>1.13917398348e-21</value>
-      <value>-5.88077563059e-22</value>
-      <value>-6.46942759641e-22</value>
-      <value>1.24155761140e-21</value>
-      <value>-2.39767595884e-21</value>
-      <value>-1.92529838027e-21</value>
-      <value>-2.67276061117e-21</value>
-      <value>-3.71878163754e-22</value>
-      <value>2.93286555809e-21</value>
-      <value>5.95216366683e-21</value>
-      <value>2.23824499224e-21</value>
-      <value>-2.37025360220e-21</value>
-      <value>2.51115976383e-21</value>
-      <value>4.41839049227e-21</value>
-      <value>-4.24657218566e-21</value>
-      <value>-7.40619035814e-22</value>
-      <value>2.21162169361e-21</value>
-      <value>-3.48135871731e-21</value>
-      <value>-3.38260757309e-22</value>
-      <value>8.74242467199e-22</value>
-      <value>1.24222114875e-21</value>
-      <value>2.88320864191e-22</value>
-      <value>-3.89514078871e-23</value>
-      <value>2.03926751714e-22</value>
-      <value>-2.44408757800e-22</value>
-      <value>-1.19000091496e-21</value>
-      <value>-4.46535895578e-22</value>
-      <value>2.63820518696e-21</value>
-      <value>-3.93853976946e-21</value>
-      <value>2.16159418495e-21</value>
-      <value>5.75427109211e-21</value>
-      <value>6.01177217041e-21</value>
-      <value>6.33825663125e-21</value>
-      <value>-5.39641371675e-21</value>
-      <value>-2.58853553846e-21</value>
-      <value>-2.41520518642e-23</value>
-      <value>1.10077206512e-21</value>
-      <value>-1.03118036508e-21</value>
-      <value>1.68793531323e-20</value>
-      <value>4.10819950273e-21</value>
-      <value>4.10689206219e-21</value>
-      <value>-1.02367789006e-22</value>
-      <value>1.76548176324e-21</value>
-      <value>-1.03789483989e-21</value>
-      <value>1.38183428860e-21</value>
-      <value>1.01900334868e-21</value>
-      <value>5.37306364583e-21</value>
-      <value>2.31566523144e-21</value>
-      <value>-3.78975043130e-21</value>
-      <value>2.26173975440e-21</value>
-      <value>9.53493292883e-22</value>
-      <value>-8.59906247961e-23</value>
-      <value>-8.50535104636e-22</value>
-      <value>5.72665267797e-22</value>
-      <value>-4.60167553622e-22</value>
-      <value>-8.99424233859e-22</value>
-      <value>-1.11883634805e-21</value>
-      <value>1.65468300943e-22</value>
-      <value>8.85075696970e-22</value>
-      <value>-1.68469270162e-22</value>
-      <value>1.89091540129e-21</value>
-      <value>-1.49242970343e-21</value>
-      <value>1.18198737437e-21</value>
-      <value>-6.70186247556e-22</value>
-      <value>-1.97814269267e-22</value>
-      <value>-5.71375597836e-22</value>
-      <value>1.81628646939e-21</value>
-      <value>-1.58848721366e-22</value>
-      <value>2.31679595438e-21</value>
-      <value>2.61865508386e-21</value>
-      <value>1.57860340440e-21</value>
-      <value>-3.07053933242e-22</value>
-      <value>-2.50077149073e-21</value>
-      <value>1.72697856692e-21</value>
-      <value>-2.47899981176e-22</value>
-      <value>-2.22580760015e-22</value>
-      <value>-6.14556879635e-22</value>
-      <value>-1.94268154479e-21</value>
-      <value>-8.61966159240e-22</value>
-      <value>-6.80968705666e-22</value>
-      <value>3.18273544707e-22</value>
-      <value>-4.73785770016e-21</value>
-      <value>8.82133987478e-22</value>
-      <value>-2.35802536772e-21</value>
-      <value>4.91417880826e-21</value>
-      <value>-1.83006821323e-21</value>
-      <value>-7.43451313543e-23</value>
-      <value>-6.23504389276e-22</value>
-      <value>2.56292044298e-21</value>
-      <value>6.37072177871e-21</value>
-      <value>-5.33591786218e-21</value>
-      <value>-1.04257929628e-21</value>
-      <value>2.96953376735e-21</value>
+      <value>1.54130648146e-20</value>
+      <value>-1.54735767570e-20</value>
+      <value>-1.21134748197e-21</value>
+      <value>1.80392669631e-21</value>
+      <value>-2.58241075906e-21</value>
+      <value>-1.91146172542e-21</value>
+      <value>8.11909184467e-21</value>
+      <value>7.98326743347e-22</value>
+      <value>-3.69104948053e-21</value>
+      <value>5.18682088043e-22</value>
+      <value>-7.19402543546e-21</value>
+      <value>2.96943870380e-21</value>
+      <value>-1.15806856043e-21</value>
+      <value>-8.84188161434e-22</value>
+      <value>-4.24917049383e-21</value>
+      <value>3.06270504463e-21</value>
+      <value>1.67727736030e-21</value>
+      <value>2.09757154703e-21</value>
+      <value>-8.14880717870e-22</value>
+      <value>1.49336855603e-21</value>
+      <value>1.37663870978e-21</value>
+      <value>-3.30745901633e-21</value>
+      <value>5.22724952481e-22</value>
+      <value>2.54871669800e-21</value>
+      <value>2.17703891985e-21</value>
+      <value>-2.13692917748e-21</value>
+      <value>4.26842169379e-21</value>
+      <value>2.00554953424e-21</value>
+      <value>-1.92356325773e-21</value>
+      <value>2.54955979882e-21</value>
+      <value>3.29010965879e-21</value>
+      <value>-2.93022548660e-21</value>
+      <value>-2.20421647542e-21</value>
+      <value>1.70349691405e-21</value>
+      <value>-1.27335354008e-21</value>
+      <value>1.01174913620e-21</value>
+      <value>-2.17554120698e-21</value>
+      <value>-5.47969196450e-21</value>
+      <value>-2.85608969787e-21</value>
+      <value>4.11767228309e-21</value>
+      <value>-7.15047753967e-22</value>
+      <value>2.90365236158e-21</value>
+      <value>3.49483205701e-21</value>
+      <value>9.17966532158e-22</value>
+      <value>-1.16337894305e-21</value>
+      <value>4.27126421021e-22</value>
+      <value>-2.98731527659e-21</value>
+      <value>6.95164321570e-21</value>
+      <value>3.58058969912e-21</value>
+      <value>3.66771644767e-22</value>
+      <value>-1.02848808213e-21</value>
+      <value>1.99016068606e-21</value>
+      <value>3.19486140750e-22</value>
+      <value>2.46874680654e-21</value>
+      <value>-4.15095297497e-22</value>
+      <value>1.65061511464e-20</value>
+      <value>2.29001782848e-20</value>
+      <value>-2.34271630387e-20</value>
+      <value>1.86534449351e-21</value>
+      <value>1.09255690605e-20</value>
+      <value>-4.45412304685e-22</value>
+      <value>1.26247236458e-20</value>
+      <value>-1.46917717069e-20</value>
+      <value>-1.81343019018e-20</value>
+      <value>8.63435814646e-21</value>
+      <value>1.44532142935e-20</value>
+      <value>6.12982461140e-22</value>
+      <value>-7.78456635069e-21</value>
+      <value>-2.05571174885e-21</value>
+      <value>4.73208062703e-21</value>
+      <value>-2.63838183319e-21</value>
+      <value>-2.35967409078e-22</value>
+      <value>4.69136942192e-21</value>
+      <value>8.69835967049e-21</value>
+      <value>2.17530866027e-21</value>
+      <value>-6.03772278959e-21</value>
+      <value>-1.03724370018e-21</value>
+      <value>-6.24581604401e-21</value>
+      <value>6.60334375868e-21</value>
+      <value>-2.82044788439e-21</value>
+      <value>2.47337245796e-21</value>
+      <value>-8.03401986551e-21</value>
+      <value>1.08399513730e-20</value>
+      <value>8.70672953282e-21</value>
+      <value>1.44724172555e-20</value>
+      <value>9.06115367409e-21</value>
+      <value>1.98787818057e-20</value>
+      <value>2.82784632823e-21</value>
+      <value>-1.48714217087e-20</value>
+      <value>-2.12171985494e-20</value>
+      <value>1.28819489470e-20</value>
+      <value>-2.50128416413e-20</value>
+      <value>1.40870382920e-20</value>
+      <value>-2.69541915019e-20</value>
+      <value>-1.26179291100e-20</value>
+      <value>-7.47023123926e-21</value>
+      <value>-3.89005161485e-21</value>
+      <value>-5.30078540176e-21</value>
+      <value>2.82924015295e-21</value>
+      <value>2.33980622384e-21</value>
+      <value>5.47226098144e-21</value>
+      <value>-5.32745425351e-20</value>
+      <value>1.81883796691e-20</value>
+      <value>-6.15264340707e-21</value>
+      <value>-1.15397222208e-20</value>
+      <value>-1.43319062512e-20</value>
+      <value>-5.56558757275e-20</value>
+      <value>3.80137429806e-20</value>
+      <value>1.50468536364e-20</value>
+      <value>-9.55491850318e-21</value>
     </rpSampledBases>
   </XpSampling>
   <XpMerge>
     <sampleMeanWavelengths>
-      <value>433.063</value>
-      <value>596.050</value>
-      <value>807.251</value>
+      <value>705.575</value>
+      <value>904.228</value>
     </sampleMeanWavelengths>
     <bpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
     </bpWeights>
     <rpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
     </rpWeights>
   </XpMerge>
   <fluxBias>
-    <value>5.33539e-20</value>
-    <value>3.82022e-20</value>
-    <value>1.76185e-20</value>
+    <value>0.00000</value>
+    <value>0.00000</value>
   </fluxBias>
   <zeropoints>
-    <value>-25.4227</value>
-    <value>-26.3381</value>
-    <value>-27.3352</value>
+    <value>-26.9158</value>
+    <value>-27.6789</value>
   </zeropoints>
 </config>
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_IphasCustom_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Stromgren_v375wiv142r.xml`

 * *Files 24% similar despite different names*

#### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_IphasCustom_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_Stromgren_v375wiv142r.xml`

```diff
@@ -1,720 +1,488 @@
 <?xml version="1.0" encoding="utf-8"?>
 <config>
   <solutionId>4545469030156206114</solutionId>
-  <bands n="6">
-    <item>Halpha</item>
-    <item>Hbeta</item>
-    <item>O3</item>
-    <item>CHalpha</item>
-    <item>CHbeta</item>
-    <item>CO3</item>
+  <bands n="4">
+    <item>u</item>
+    <item>v</item>
+    <item>b</item>
+    <item>y</item>
   </bands>
   <XpSampling>
     <bpSampledBases dimension="55">
-      <value>8.60336e-23</value>
-      <value>1.15147e-22</value>
-      <value>1.44514e-22</value>
-      <value>3.45003e-23</value>
-      <value>-8.36115e-23</value>
-      <value>-4.81529e-23</value>
-      <value>1.89621e-22</value>
-      <value>9.61803e-23</value>
-      <value>-8.94557e-23</value>
-      <value>-7.38832e-23</value>
-      <value>2.22815e-22</value>
-      <value>-5.41997e-23</value>
-      <value>1.47314e-22</value>
-      <value>1.13852e-22</value>
-      <value>-3.90599e-23</value>
-      <value>1.81763e-22</value>
-      <value>5.64144e-23</value>
-      <value>7.70013e-23</value>
-      <value>-6.39183e-23</value>
-      <value>2.38318e-23</value>
-      <value>-1.26420e-22</value>
-      <value>-6.40202e-23</value>
-      <value>-1.07832e-22</value>
-      <value>-4.03717e-23</value>
-      <value>1.22845e-22</value>
-      <value>-5.80854e-23</value>
-      <value>7.35551e-23</value>
-      <value>-5.52154e-23</value>
-      <value>-7.67835e-23</value>
-      <value>3.30968e-23</value>
-      <value>2.04482e-23</value>
-      <value>-2.26745e-23</value>
-      <value>-2.51463e-23</value>
-      <value>3.05639e-23</value>
-      <value>3.48600e-23</value>
-      <value>4.97717e-23</value>
-      <value>-1.36578e-23</value>
-      <value>2.91328e-23</value>
-      <value>2.48512e-24</value>
-      <value>1.76118e-23</value>
-      <value>-1.97695e-23</value>
-      <value>6.15689e-24</value>
-      <value>6.88044e-23</value>
-      <value>3.98639e-23</value>
-      <value>-1.04871e-22</value>
-      <value>3.11912e-23</value>
-      <value>4.47118e-23</value>
-      <value>1.19248e-23</value>
-      <value>-1.37410e-22</value>
-      <value>-2.79770e-24</value>
-      <value>-1.41401e-22</value>
-      <value>-8.65334e-24</value>
-      <value>1.45662e-22</value>
-      <value>2.39455e-24</value>
-      <value>3.34508e-23</value>
-      <value>2.07183e-20</value>
-      <value>-3.48042e-20</value>
-      <value>-1.16525e-20</value>
-      <value>1.07893e-20</value>
-      <value>-1.71284e-20</value>
-      <value>-5.59710e-20</value>
-      <value>-4.43491e-20</value>
-      <value>2.35387e-20</value>
-      <value>-4.77603e-20</value>
-      <value>2.12036e-20</value>
-      <value>1.06717e-20</value>
-      <value>-1.02564e-20</value>
-      <value>-1.84765e-20</value>
-      <value>1.12577e-21</value>
-      <value>1.17423e-20</value>
-      <value>4.27157e-20</value>
-      <value>-6.95270e-20</value>
-      <value>-4.16258e-20</value>
-      <value>4.76696e-20</value>
-      <value>1.73108e-20</value>
-      <value>-5.10939e-20</value>
-      <value>-3.48792e-21</value>
-      <value>-1.70905e-20</value>
-      <value>-3.73741e-20</value>
-      <value>-1.57996e-20</value>
-      <value>1.99430e-20</value>
-      <value>-2.00143e-20</value>
-      <value>4.44275e-21</value>
-      <value>3.15824e-20</value>
-      <value>-2.04030e-20</value>
-      <value>6.32085e-21</value>
-      <value>-1.01611e-20</value>
-      <value>7.00502e-21</value>
-      <value>-3.97684e-20</value>
-      <value>-7.87950e-21</value>
-      <value>-3.00922e-21</value>
-      <value>2.31858e-21</value>
-      <value>-4.24418e-21</value>
-      <value>-1.84466e-20</value>
-      <value>-2.25739e-20</value>
-      <value>7.41122e-21</value>
-      <value>-1.20533e-20</value>
-      <value>-5.29622e-20</value>
-      <value>-9.86268e-21</value>
-      <value>1.10030e-20</value>
-      <value>-4.77466e-20</value>
-      <value>2.18511e-20</value>
-      <value>5.75763e-21</value>
-      <value>-1.31924e-20</value>
-      <value>4.80513e-21</value>
-      <value>2.60232e-21</value>
-      <value>2.91534e-21</value>
-      <value>2.03999e-20</value>
-      <value>-4.33530e-21</value>
-      <value>1.25676e-20</value>
-      <value>2.07071e-20</value>
-      <value>-3.11354e-20</value>
-      <value>2.26992e-21</value>
-      <value>2.71711e-20</value>
-      <value>-5.66672e-20</value>
-      <value>-6.24307e-22</value>
-      <value>-3.17508e-20</value>
-      <value>5.48894e-21</value>
-      <value>-7.22601e-21</value>
-      <value>2.84427e-20</value>
-      <value>1.09987e-20</value>
-      <value>8.98525e-21</value>
-      <value>-3.13324e-20</value>
-      <value>5.02146e-21</value>
-      <value>1.07223e-20</value>
-      <value>3.60249e-20</value>
-      <value>-1.60674e-20</value>
-      <value>2.51028e-21</value>
-      <value>-3.78067e-20</value>
-      <value>-2.09070e-20</value>
-      <value>9.16945e-20</value>
-      <value>2.50235e-20</value>
-      <value>-2.94561e-21</value>
-      <value>-1.66409e-20</value>
-      <value>4.22160e-20</value>
-      <value>-2.36846e-20</value>
-      <value>1.83585e-20</value>
-      <value>-4.68024e-21</value>
-      <value>-2.85256e-20</value>
-      <value>1.21390e-20</value>
-      <value>7.51756e-22</value>
-      <value>-5.87038e-21</value>
-      <value>-6.91579e-21</value>
-      <value>1.78804e-20</value>
-      <value>8.89067e-21</value>
-      <value>8.56514e-21</value>
-      <value>-9.02077e-21</value>
-      <value>3.78223e-21</value>
-      <value>1.08197e-20</value>
-      <value>1.46333e-20</value>
-      <value>-2.64829e-21</value>
-      <value>5.68186e-21</value>
-      <value>3.54933e-20</value>
-      <value>1.15848e-20</value>
-      <value>-2.55374e-20</value>
-      <value>3.75171e-20</value>
-      <value>3.80182e-21</value>
-      <value>1.02668e-21</value>
-      <value>-9.99269e-21</value>
-      <value>-8.05058e-21</value>
-      <value>-2.20026e-20</value>
-      <value>-4.46450e-21</value>
-      <value>2.03443e-21</value>
-      <value>2.56976e-21</value>
-      <value>-4.51032e-21</value>
-      <value>2.35538e-20</value>
-      <value>2.74921e-20</value>
-      <value>2.66335e-20</value>
-      <value>-5.27850e-21</value>
-      <value>-4.19677e-20</value>
-      <value>-9.46858e-21</value>
-      <value>4.57255e-20</value>
-      <value>1.56882e-20</value>
-      <value>-3.08966e-20</value>
-      <value>-5.63524e-20</value>
-      <value>4.41350e-20</value>
-      <value>-4.30513e-20</value>
-      <value>2.80895e-20</value>
-      <value>4.18170e-20</value>
-      <value>-2.59480e-20</value>
-      <value>3.84027e-20</value>
-      <value>1.95416e-20</value>
-      <value>-2.33997e-20</value>
-      <value>-2.02721e-20</value>
-      <value>1.36707e-20</value>
-      <value>-2.74541e-20</value>
-      <value>-1.68891e-20</value>
-      <value>-3.31054e-20</value>
-      <value>3.44257e-22</value>
-      <value>1.85278e-20</value>
-      <value>1.49199e-20</value>
-      <value>1.24667e-20</value>
-      <value>-1.63162e-20</value>
-      <value>-2.79999e-20</value>
-      <value>-1.01977e-21</value>
-      <value>-7.94385e-21</value>
-      <value>2.48375e-21</value>
-      <value>-6.78321e-21</value>
-      <value>1.49989e-20</value>
-      <value>2.40482e-21</value>
-      <value>7.61916e-21</value>
-      <value>-1.84537e-21</value>
-      <value>7.18477e-21</value>
-      <value>1.17961e-20</value>
-      <value>1.21296e-20</value>
-      <value>-5.36896e-21</value>
-      <value>9.37144e-21</value>
-      <value>3.36089e-20</value>
-      <value>1.41835e-20</value>
-      <value>-2.75436e-20</value>
-      <value>1.95909e-20</value>
-      <value>1.09951e-20</value>
-      <value>-5.35901e-21</value>
-      <value>-3.31449e-20</value>
-      <value>-9.23166e-21</value>
-      <value>-3.75735e-20</value>
-      <value>-3.11115e-21</value>
-      <value>3.10992e-20</value>
-      <value>1.12069e-20</value>
-      <value>-3.58875e-21</value>
-      <value>2.10936e-20</value>
-      <value>-4.35396e-20</value>
-      <value>2.47342e-21</value>
-      <value>-1.16841e-20</value>
-      <value>5.85746e-20</value>
-      <value>-8.66055e-20</value>
-      <value>2.29366e-20</value>
-      <value>1.91389e-21</value>
-      <value>1.02963e-21</value>
-      <value>-2.86583e-20</value>
-      <value>-1.77765e-20</value>
-      <value>9.41230e-21</value>
-      <value>1.96339e-20</value>
-      <value>-5.95753e-21</value>
-      <value>-1.70795e-20</value>
-      <value>-5.87819e-20</value>
-      <value>4.57052e-20</value>
-      <value>4.65550e-20</value>
-      <value>-6.96617e-20</value>
-      <value>2.91435e-20</value>
-      <value>2.87152e-20</value>
-      <value>2.61719e-20</value>
-      <value>-2.84920e-20</value>
-      <value>9.92778e-22</value>
-      <value>2.23314e-20</value>
-      <value>9.56702e-20</value>
-      <value>3.30397e-20</value>
-      <value>3.16123e-20</value>
-      <value>6.32681e-20</value>
-      <value>-1.71198e-20</value>
-      <value>2.55275e-20</value>
-      <value>-6.27907e-21</value>
-      <value>1.10346e-20</value>
-      <value>-3.94511e-20</value>
-      <value>-1.27414e-20</value>
-      <value>-5.36317e-21</value>
-      <value>-7.05234e-21</value>
-      <value>-4.14024e-21</value>
-      <value>-1.73823e-20</value>
-      <value>-1.32729e-20</value>
-      <value>2.20017e-21</value>
-      <value>-1.10572e-20</value>
-      <value>-3.52013e-20</value>
-      <value>-1.48803e-20</value>
-      <value>3.13124e-20</value>
-      <value>9.51038e-22</value>
-      <value>-3.85849e-20</value>
-      <value>2.54078e-20</value>
-      <value>2.73210e-20</value>
-      <value>2.63978e-20</value>
-      <value>2.97174e-20</value>
-      <value>1.16667e-20</value>
-      <value>1.61606e-21</value>
-      <value>-8.98827e-21</value>
-      <value>1.52364e-20</value>
-      <value>2.26174e-20</value>
-      <value>-1.69021e-20</value>
-      <value>3.92229e-21</value>
-      <value>5.04396e-20</value>
-      <value>-1.93715e-20</value>
-      <value>3.92327e-20</value>
-      <value>1.24179e-20</value>
-      <value>-5.39642e-21</value>
-      <value>3.06541e-21</value>
-      <value>-1.98529e-20</value>
-      <value>-3.12039e-21</value>
-      <value>3.58173e-21</value>
-      <value>3.18304e-20</value>
-      <value>2.65206e-21</value>
-      <value>-3.45745e-20</value>
-      <value>-3.50508e-20</value>
-      <value>2.40321e-21</value>
-      <value>-2.24603e-20</value>
-      <value>1.35087e-20</value>
-      <value>1.99378e-20</value>
-      <value>-1.55045e-20</value>
-      <value>7.54350e-21</value>
-      <value>1.22121e-20</value>
-      <value>1.36203e-20</value>
-      <value>-3.22506e-20</value>
-      <value>3.11364e-20</value>
-      <value>-1.37067e-20</value>
-      <value>1.39299e-20</value>
-      <value>2.30568e-20</value>
-      <value>-1.06059e-20</value>
-      <value>-1.33256e-20</value>
-      <value>1.17699e-20</value>
-      <value>8.53624e-21</value>
-      <value>-9.85884e-21</value>
-      <value>-1.02098e-20</value>
-      <value>-1.60734e-20</value>
-      <value>1.09312e-20</value>
-      <value>-4.76145e-21</value>
-      <value>-8.10465e-21</value>
-      <value>-7.44732e-21</value>
-      <value>4.77750e-21</value>
-      <value>8.43615e-22</value>
-      <value>-2.94553e-20</value>
-      <value>-1.79351e-20</value>
-      <value>4.39656e-20</value>
-      <value>-3.11393e-20</value>
-      <value>-2.58585e-20</value>
-      <value>-1.19465e-21</value>
-      <value>4.35300e-20</value>
-      <value>1.08063e-20</value>
-      <value>4.83143e-20</value>
-      <value>8.69108e-21</value>
-      <value>-3.69962e-20</value>
-      <value>-1.64015e-21</value>
-      <value>-5.38584e-21</value>
+      <value>9.33782382157e-21</value>
+      <value>-3.58692954997e-20</value>
+      <value>5.70227509367e-20</value>
+      <value>-7.87210689822e-20</value>
+      <value>9.74868410085e-20</value>
+      <value>1.73176761795e-19</value>
+      <value>-1.06341252166e-19</value>
+      <value>1.13335587192e-19</value>
+      <value>-4.88586237188e-19</value>
+      <value>1.60690498832e-20</value>
+      <value>-1.49794044220e-19</value>
+      <value>3.66648565194e-20</value>
+      <value>1.27148000704e-19</value>
+      <value>3.06913784172e-20</value>
+      <value>4.72507165876e-21</value>
+      <value>-1.51273220936e-20</value>
+      <value>1.79908316549e-19</value>
+      <value>-9.72163625636e-21</value>
+      <value>-4.73313907203e-20</value>
+      <value>-1.83528078563e-19</value>
+      <value>6.87200577886e-20</value>
+      <value>-2.42844007965e-20</value>
+      <value>-3.28111799064e-19</value>
+      <value>1.44098373023e-19</value>
+      <value>1.64352830658e-19</value>
+      <value>-3.20769953569e-19</value>
+      <value>-3.22229384266e-19</value>
+      <value>1.14812132065e-19</value>
+      <value>1.98921779431e-19</value>
+      <value>-6.05819374946e-19</value>
+      <value>-5.02965737322e-20</value>
+      <value>2.32921756004e-19</value>
+      <value>-2.79979707064e-19</value>
+      <value>2.02243806551e-19</value>
+      <value>3.40676809468e-19</value>
+      <value>-7.76576196489e-20</value>
+      <value>-5.11999364313e-19</value>
+      <value>1.77106655328e-19</value>
+      <value>5.85149534915e-19</value>
+      <value>-2.09266955061e-19</value>
+      <value>-1.02391872364e-18</value>
+      <value>3.03837586742e-19</value>
+      <value>-2.99165164727e-19</value>
+      <value>4.24636436689e-19</value>
+      <value>-2.44980408325e-19</value>
+      <value>-2.97806069457e-19</value>
+      <value>-2.65886236223e-19</value>
+      <value>6.77871756590e-19</value>
+      <value>-3.09698116673e-19</value>
+      <value>1.78560064988e-19</value>
+      <value>5.28617202558e-19</value>
+      <value>6.36116143792e-20</value>
+      <value>4.87077347512e-19</value>
+      <value>-6.97395422793e-20</value>
+      <value>5.59108077511e-20</value>
+      <value>1.55660857131e-20</value>
+      <value>-5.61665402917e-20</value>
+      <value>7.50348475099e-20</value>
+      <value>-5.96331699093e-20</value>
+      <value>2.63751230726e-21</value>
+      <value>4.34983904371e-20</value>
+      <value>5.17182906784e-21</value>
+      <value>-1.32842341805e-20</value>
+      <value>2.20854427518e-20</value>
+      <value>2.53143903452e-20</value>
+      <value>1.09612543897e-20</value>
+      <value>-1.96930703983e-20</value>
+      <value>-1.17191761936e-20</value>
+      <value>-2.86403777930e-20</value>
+      <value>3.53980462192e-20</value>
+      <value>5.28064175006e-20</value>
+      <value>-3.60902047429e-20</value>
+      <value>-2.50637840995e-20</value>
+      <value>-3.72268864852e-20</value>
+      <value>-8.98682999555e-20</value>
+      <value>-1.28515878107e-19</value>
+      <value>2.30676121424e-19</value>
+      <value>-2.75447652492e-20</value>
+      <value>1.22306493404e-19</value>
+      <value>-6.29755945442e-21</value>
+      <value>7.34019240128e-21</value>
+      <value>6.91986155765e-20</value>
+      <value>1.21143238872e-20</value>
+      <value>3.01648977124e-20</value>
+      <value>2.96892796344e-20</value>
+      <value>2.07841567396e-20</value>
+      <value>2.04586132094e-20</value>
+      <value>-1.41394450664e-20</value>
+      <value>4.42708197378e-20</value>
+      <value>1.78552364949e-20</value>
+      <value>3.06037861286e-20</value>
+      <value>3.96064179934e-20</value>
+      <value>-6.48734195448e-20</value>
+      <value>-8.59542515223e-21</value>
+      <value>1.25233921311e-20</value>
+      <value>6.61636785040e-21</value>
+      <value>6.30197680030e-20</value>
+      <value>-4.15883550675e-20</value>
+      <value>-5.28618711743e-20</value>
+      <value>3.79939937440e-20</value>
+      <value>-6.96762732377e-20</value>
+      <value>-4.86072804073e-20</value>
+      <value>4.62065407437e-20</value>
+      <value>-9.56976155332e-20</value>
+      <value>-3.23011064162e-22</value>
+      <value>-1.23794058411e-19</value>
+      <value>-7.14668027970e-21</value>
+      <value>1.12912168251e-19</value>
+      <value>2.66447430624e-20</value>
+      <value>3.99020008761e-20</value>
+      <value>2.13138380531e-20</value>
+      <value>-4.13264375620e-20</value>
+      <value>-6.33255302372e-21</value>
+      <value>-7.28871305104e-21</value>
+      <value>3.73030881568e-20</value>
+      <value>-8.52441123432e-20</value>
+      <value>2.18465479714e-21</value>
+      <value>7.82471844070e-21</value>
+      <value>-1.12795939001e-20</value>
+      <value>-1.08985163118e-20</value>
+      <value>-8.48497330066e-21</value>
+      <value>5.14692569020e-21</value>
+      <value>6.91420313126e-21</value>
+      <value>-7.08355929668e-21</value>
+      <value>-1.22081712610e-20</value>
+      <value>-1.82198104468e-20</value>
+      <value>1.71302255008e-20</value>
+      <value>2.42568973473e-20</value>
+      <value>-8.13746560281e-20</value>
+      <value>2.15245811039e-20</value>
+      <value>-3.60096164558e-20</value>
+      <value>-3.62792024818e-20</value>
+      <value>9.11191755429e-20</value>
+      <value>7.44842408584e-20</value>
+      <value>4.89677308711e-20</value>
+      <value>-1.16751689338e-20</value>
+      <value>3.59243282661e-21</value>
+      <value>-2.46052399233e-20</value>
+      <value>-4.05085406723e-20</value>
+      <value>-4.96383242908e-22</value>
+      <value>-2.62555863026e-20</value>
+      <value>1.73847872134e-20</value>
+      <value>-1.14343012949e-20</value>
+      <value>3.48560633574e-20</value>
+      <value>8.57895110311e-21</value>
+      <value>-1.93240717747e-21</value>
+      <value>4.36692092755e-21</value>
+      <value>9.42760304624e-21</value>
+      <value>1.96210841787e-20</value>
+      <value>5.56908628161e-21</value>
+      <value>-7.25922209714e-22</value>
+      <value>1.78920987270e-20</value>
+      <value>2.01253243616e-20</value>
+      <value>1.89559677952e-20</value>
+      <value>-3.02256603598e-20</value>
+      <value>1.52446759829e-21</value>
+      <value>3.82389346072e-20</value>
+      <value>-1.97157333356e-20</value>
+      <value>-2.78783596915e-20</value>
+      <value>-2.43801235474e-20</value>
+      <value>-2.97568755039e-20</value>
+      <value>-1.03728574618e-20</value>
+      <value>6.95206714670e-21</value>
+      <value>7.37639919168e-21</value>
+      <value>-1.17974630296e-20</value>
+      <value>2.44126120428e-20</value>
+      <value>-8.01145971227e-21</value>
+      <value>-1.72432037044e-20</value>
+      <value>3.12747415393e-20</value>
+      <value>2.77823791055e-20</value>
+      <value>2.43402401915e-20</value>
+      <value>2.91613356603e-20</value>
+      <value>-6.34043739002e-21</value>
+      <value>1.09013708285e-21</value>
+      <value>-5.45957925186e-20</value>
+      <value>8.70503042021e-21</value>
+      <value>6.09505598087e-20</value>
+      <value>4.82001351307e-20</value>
+      <value>-2.26785237438e-20</value>
+      <value>8.44547722036e-22</value>
+      <value>1.07510627999e-19</value>
+      <value>6.21648576799e-20</value>
+      <value>-6.95887279033e-20</value>
+      <value>6.04229511140e-22</value>
+      <value>5.41938757231e-20</value>
+      <value>-1.76286013057e-20</value>
+      <value>-4.95783808304e-21</value>
+      <value>-1.59558912305e-20</value>
+      <value>6.55170507289e-21</value>
+      <value>-2.33035971624e-20</value>
+      <value>5.22049662574e-20</value>
+      <value>-1.93682752078e-20</value>
+      <value>2.01208081637e-21</value>
+      <value>-8.16927975593e-22</value>
+      <value>-1.20054653877e-20</value>
+      <value>-2.90583375030e-20</value>
+      <value>1.87114158276e-20</value>
+      <value>5.83410451552e-21</value>
+      <value>1.42434226059e-20</value>
+      <value>-1.43651507647e-20</value>
+      <value>-1.87050005696e-20</value>
+      <value>7.86560982311e-21</value>
+      <value>1.32180354929e-21</value>
+      <value>8.74930751782e-21</value>
+      <value>1.15322170908e-20</value>
+      <value>4.01858919663e-21</value>
+      <value>1.41922854545e-20</value>
+      <value>1.45458608641e-20</value>
+      <value>-2.68955023266e-21</value>
+      <value>2.17922036443e-20</value>
+      <value>6.43267725162e-21</value>
+      <value>-2.02676704769e-20</value>
+      <value>-1.00661551810e-20</value>
+      <value>3.01383979541e-20</value>
+      <value>-3.68198263960e-21</value>
+      <value>2.42023934987e-20</value>
+      <value>1.74558094087e-21</value>
+      <value>-4.02700610437e-20</value>
+      <value>1.16169129358e-20</value>
+      <value>-2.30727201105e-20</value>
     </bpSampledBases>
     <rpSampledBases dimension="55">
-      <value>1.72473e-20</value>
-      <value>-2.83303e-20</value>
-      <value>-1.37416e-20</value>
-      <value>-2.03533e-20</value>
-      <value>1.49018e-20</value>
-      <value>4.68295e-20</value>
-      <value>3.62402e-20</value>
-      <value>4.37143e-20</value>
-      <value>-2.32049e-20</value>
-      <value>-8.39528e-21</value>
-      <value>-2.62055e-21</value>
-      <value>-6.88469e-20</value>
-      <value>6.58423e-22</value>
-      <value>4.29009e-20</value>
-      <value>-6.78116e-20</value>
-      <value>2.06614e-22</value>
-      <value>-1.03860e-20</value>
-      <value>-4.72897e-21</value>
-      <value>-3.34519e-20</value>
-      <value>1.50487e-20</value>
-      <value>-3.79536e-20</value>
-      <value>1.28846e-20</value>
-      <value>1.92573e-20</value>
-      <value>3.18662e-20</value>
-      <value>1.29541e-20</value>
-      <value>2.62929e-20</value>
-      <value>-3.26794e-20</value>
-      <value>-3.89164e-20</value>
-      <value>2.60301e-20</value>
-      <value>1.85728e-20</value>
-      <value>-3.61209e-20</value>
-      <value>1.37488e-20</value>
-      <value>2.31880e-20</value>
-      <value>-2.52964e-20</value>
-      <value>1.74270e-20</value>
-      <value>-6.07755e-21</value>
-      <value>-3.66032e-21</value>
-      <value>-2.06989e-20</value>
-      <value>-5.37959e-21</value>
-      <value>8.73160e-21</value>
-      <value>-1.94475e-21</value>
-      <value>2.42811e-21</value>
-      <value>-2.92636e-21</value>
-      <value>-2.38529e-21</value>
-      <value>1.18027e-20</value>
-      <value>-1.59843e-20</value>
-      <value>6.69545e-21</value>
-      <value>1.00460e-20</value>
-      <value>1.50618e-20</value>
-      <value>1.90118e-20</value>
-      <value>-2.95994e-21</value>
-      <value>-1.06437e-21</value>
-      <value>-2.10234e-21</value>
-      <value>-4.55805e-21</value>
-      <value>-1.49887e-21</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>3.25818e-21</value>
-      <value>-6.34913e-21</value>
-      <value>-6.63033e-21</value>
-      <value>-6.27048e-21</value>
-      <value>-4.57778e-21</value>
-      <value>1.11232e-20</value>
-      <value>-2.40476e-21</value>
-      <value>-7.07377e-21</value>
-      <value>6.93675e-21</value>
-      <value>-3.52990e-21</value>
-      <value>3.36463e-21</value>
-      <value>5.70140e-21</value>
-      <value>-1.01184e-20</value>
-      <value>-1.14389e-20</value>
-      <value>9.26144e-22</value>
-      <value>-3.62498e-21</value>
-      <value>6.88739e-21</value>
-      <value>1.28112e-20</value>
-      <value>1.64319e-20</value>
-      <value>-9.50761e-21</value>
-      <value>2.19541e-20</value>
-      <value>2.34899e-21</value>
-      <value>3.04443e-21</value>
-      <value>-4.33797e-21</value>
-      <value>-3.22188e-22</value>
-      <value>-1.02126e-20</value>
-      <value>-2.07838e-20</value>
-      <value>-1.70297e-20</value>
-      <value>-2.54989e-20</value>
-      <value>1.78156e-20</value>
-      <value>1.16946e-20</value>
-      <value>-7.89445e-21</value>
-      <value>4.39563e-20</value>
-      <value>-4.40255e-20</value>
-      <value>3.66537e-20</value>
-      <value>9.67187e-22</value>
-      <value>-2.37319e-20</value>
-      <value>-4.00335e-20</value>
-      <value>-1.21917e-21</value>
-      <value>-1.94073e-21</value>
-      <value>2.20838e-21</value>
-      <value>-7.07675e-21</value>
-      <value>-4.65139e-20</value>
-      <value>-1.05521e-20</value>
-      <value>1.84117e-20</value>
-      <value>1.29154e-20</value>
-      <value>-2.84328e-21</value>
-      <value>-2.96993e-20</value>
-      <value>2.61806e-20</value>
-      <value>9.72061e-21</value>
-      <value>1.73519e-20</value>
-      <value>1.30046e-20</value>
-      <value>-3.64666e-21</value>
-      <value>-8.94066e-21</value>
-      <value>1.20402e-21</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
     </rpSampledBases>
   </XpSampling>
   <XpMerge>
     <sampleMeanWavelengths>
-      <value>656.300</value>
-      <value>486.100</value>
-      <value>500.700</value>
-      <value>635.000</value>
-      <value>460.000</value>
-      <value>530.000</value>
+      <value>347.877</value>
+      <value>410.570</value>
+      <value>469.584</value>
+      <value>550.272</value>
     </sampleMeanWavelengths>
     <bpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
-      <value>1.00000</value>
     </bpWeights>
     <rpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
-      <value>1.00000</value>
     </rpWeights>
   </XpMerge>
   <fluxBias>
     <value>0.00000</value>
     <value>0.00000</value>
     <value>0.00000</value>
     <value>0.00000</value>
-    <value>0.00000</value>
-    <value>0.00000</value>
   </fluxBias>
   <zeropoints>
-    <value>-26.7793</value>
-    <value>-25.8082</value>
-    <value>-25.8307</value>
-    <value>-26.5729</value>
-    <value>-25.5384</value>
-    <value>-25.9860</value>
+    <value>-26.2346</value>
+    <value>-25.3302</value>
+    <value>-25.6020</value>
+    <value>-26.1045</value>
   </zeropoints>
 </config>
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_JkcStd_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HipparcosTycho_v375wiv142r.xml`

 * *Files 23% similar despite different names*

#### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_JkcStd_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_HipparcosTycho_v375wiv142r.xml`

```diff
@@ -1,604 +1,372 @@
 <?xml version="1.0" encoding="utf-8"?>
 <config>
   <solutionId>4545469030156206114</solutionId>
-  <bands n="5">
-    <item>U</item>
-    <item>B</item>
-    <item>V</item>
-    <item>R</item>
-    <item>I</item>
+  <bands n="3">
+    <item>Hp</item>
+    <item>BT</item>
+    <item>VT</item>
   </bands>
   <XpSampling>
     <bpSampledBases dimension="55">
-      <value>9.82030e-21</value>
-      <value>-4.10339e-20</value>
-      <value>6.85509e-20</value>
-      <value>-7.98360e-20</value>
-      <value>9.47956e-20</value>
-      <value>1.73094e-19</value>
-      <value>-6.93395e-20</value>
-      <value>7.93214e-20</value>
-      <value>-3.75565e-19</value>
-      <value>2.84497e-20</value>
-      <value>-1.02006e-19</value>
-      <value>2.76407e-20</value>
-      <value>4.58711e-20</value>
-      <value>2.67903e-20</value>
-      <value>-5.52440e-21</value>
-      <value>-1.10704e-20</value>
-      <value>9.84513e-20</value>
-      <value>-4.67988e-21</value>
-      <value>-7.19914e-20</value>
-      <value>-7.65080e-20</value>
-      <value>4.22501e-21</value>
-      <value>-6.08652e-20</value>
-      <value>-1.18755e-19</value>
-      <value>1.72186e-20</value>
-      <value>6.13243e-20</value>
-      <value>-1.62440e-19</value>
-      <value>-1.29095e-19</value>
-      <value>2.83957e-19</value>
-      <value>-9.65092e-22</value>
-      <value>-2.82730e-19</value>
-      <value>-6.02941e-21</value>
-      <value>5.70069e-20</value>
-      <value>-1.92042e-19</value>
-      <value>7.73259e-20</value>
-      <value>9.57734e-20</value>
-      <value>-5.93640e-21</value>
-      <value>-2.32804e-19</value>
-      <value>1.42654e-19</value>
-      <value>2.60283e-19</value>
-      <value>-1.07280e-19</value>
-      <value>-5.08068e-19</value>
-      <value>1.55754e-19</value>
-      <value>-1.47685e-19</value>
-      <value>2.01057e-19</value>
-      <value>-1.64799e-19</value>
-      <value>-1.50619e-19</value>
-      <value>-1.64164e-19</value>
-      <value>3.94833e-19</value>
-      <value>-8.36571e-20</value>
-      <value>5.51785e-21</value>
-      <value>3.20003e-19</value>
-      <value>3.55842e-20</value>
-      <value>2.44204e-19</value>
-      <value>-6.98976e-20</value>
-      <value>2.24691e-20</value>
-      <value>1.74186e-20</value>
-      <value>-4.68804e-20</value>
-      <value>3.70378e-20</value>
-      <value>-3.46119e-20</value>
-      <value>1.66701e-20</value>
-      <value>5.67285e-21</value>
-      <value>1.01908e-20</value>
-      <value>-5.64862e-21</value>
-      <value>8.32260e-21</value>
-      <value>-1.10154e-21</value>
-      <value>4.44428e-21</value>
-      <value>4.90500e-21</value>
-      <value>-1.21052e-20</value>
-      <value>1.16338e-21</value>
-      <value>-6.19519e-21</value>
-      <value>5.65915e-21</value>
-      <value>-2.71185e-20</value>
-      <value>2.36416e-21</value>
-      <value>-1.29402e-20</value>
-      <value>1.86947e-20</value>
-      <value>-3.12191e-22</value>
-      <value>-8.37813e-21</value>
-      <value>-7.02324e-21</value>
-      <value>7.51450e-21</value>
-      <value>-8.47201e-21</value>
-      <value>1.98858e-21</value>
-      <value>-2.08481e-21</value>
-      <value>5.82086e-21</value>
-      <value>-3.62045e-21</value>
-      <value>1.61330e-21</value>
-      <value>-5.93194e-21</value>
-      <value>-5.22522e-21</value>
-      <value>3.70653e-21</value>
-      <value>5.29993e-22</value>
-      <value>9.90288e-21</value>
-      <value>4.78796e-21</value>
-      <value>-6.13057e-21</value>
-      <value>-4.00429e-21</value>
-      <value>-2.50711e-21</value>
-      <value>-3.98529e-21</value>
-      <value>-1.05715e-21</value>
-      <value>-1.62677e-21</value>
-      <value>-9.46032e-22</value>
-      <value>-1.55137e-21</value>
-      <value>-2.45281e-21</value>
-      <value>-3.94501e-23</value>
-      <value>1.25622e-21</value>
-      <value>-2.66292e-21</value>
-      <value>9.01115e-22</value>
-      <value>1.23129e-21</value>
-      <value>4.65454e-22</value>
-      <value>3.17554e-22</value>
-      <value>-2.58774e-22</value>
-      <value>-3.22423e-22</value>
-      <value>5.93461e-22</value>
-      <value>2.33451e-20</value>
-      <value>-8.64688e-21</value>
-      <value>-1.12068e-20</value>
-      <value>1.79067e-20</value>
-      <value>-6.81814e-21</value>
-      <value>1.92760e-20</value>
-      <value>3.62864e-21</value>
-      <value>-3.09440e-21</value>
-      <value>3.21488e-21</value>
-      <value>1.65550e-22</value>
-      <value>-2.18558e-21</value>
-      <value>-5.89278e-22</value>
-      <value>2.85085e-21</value>
-      <value>8.99830e-22</value>
-      <value>-2.86301e-21</value>
-      <value>-7.86353e-21</value>
-      <value>9.65777e-22</value>
-      <value>1.45442e-21</value>
-      <value>-4.67049e-23</value>
-      <value>-3.99320e-22</value>
-      <value>1.37915e-22</value>
-      <value>1.42795e-21</value>
-      <value>-3.69074e-22</value>
-      <value>2.05285e-21</value>
-      <value>-1.20294e-21</value>
-      <value>1.59588e-21</value>
-      <value>6.98719e-22</value>
-      <value>6.82574e-22</value>
-      <value>3.64123e-22</value>
-      <value>-3.89344e-22</value>
-      <value>-3.42352e-22</value>
-      <value>5.40216e-22</value>
-      <value>7.25399e-23</value>
-      <value>-1.39095e-22</value>
-      <value>-3.24420e-22</value>
-      <value>-4.69361e-22</value>
-      <value>4.06514e-22</value>
-      <value>-3.14437e-22</value>
-      <value>-2.63281e-22</value>
-      <value>-1.16591e-22</value>
-      <value>-2.64393e-23</value>
-      <value>3.64742e-23</value>
-      <value>-7.44057e-22</value>
-      <value>-5.36732e-22</value>
-      <value>1.44694e-21</value>
-      <value>-7.49926e-22</value>
-      <value>-9.06915e-22</value>
-      <value>-2.69839e-22</value>
-      <value>1.73393e-21</value>
-      <value>2.36675e-22</value>
-      <value>1.70335e-21</value>
-      <value>4.58024e-22</value>
-      <value>-1.61653e-21</value>
-      <value>8.96539e-23</value>
-      <value>-3.75239e-22</value>
-      <value>1.17269e-20</value>
-      <value>5.04763e-21</value>
-      <value>-9.95409e-21</value>
-      <value>-1.17597e-20</value>
-      <value>-3.29487e-21</value>
-      <value>1.18442e-21</value>
-      <value>7.32333e-22</value>
-      <value>-2.82738e-22</value>
-      <value>-1.10303e-21</value>
-      <value>-1.34749e-21</value>
-      <value>6.57140e-22</value>
-      <value>-7.32294e-21</value>
-      <value>-3.76210e-21</value>
-      <value>3.21400e-21</value>
-      <value>-2.76594e-21</value>
-      <value>-5.51676e-21</value>
-      <value>-1.61008e-21</value>
-      <value>-3.18431e-21</value>
-      <value>-4.44254e-22</value>
-      <value>-1.46163e-21</value>
-      <value>2.80315e-21</value>
-      <value>1.36259e-21</value>
-      <value>1.13288e-21</value>
-      <value>1.41757e-21</value>
-      <value>-2.01845e-21</value>
-      <value>1.33982e-21</value>
-      <value>-2.70667e-22</value>
-      <value>4.16607e-22</value>
-      <value>7.74094e-22</value>
-      <value>-5.14713e-22</value>
-      <value>-4.17438e-22</value>
-      <value>3.41726e-22</value>
-      <value>1.28431e-22</value>
-      <value>-6.11252e-22</value>
-      <value>-5.05891e-22</value>
-      <value>-2.98896e-22</value>
-      <value>3.27025e-22</value>
-      <value>-3.64631e-22</value>
-      <value>1.68925e-22</value>
-      <value>-3.94591e-22</value>
-      <value>-1.63309e-24</value>
-      <value>-2.33837e-22</value>
-      <value>-7.50912e-22</value>
-      <value>-3.61758e-22</value>
-      <value>1.08149e-21</value>
-      <value>-5.84771e-22</value>
-      <value>-2.32411e-22</value>
-      <value>-2.80976e-22</value>
-      <value>1.10002e-21</value>
-      <value>-7.59840e-23</value>
-      <value>1.24973e-21</value>
-      <value>3.28389e-22</value>
-      <value>-7.79710e-22</value>
-      <value>3.71370e-22</value>
-      <value>-4.37446e-22</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
+      <value>1.72913118126e-20</value>
+      <value>-1.54390380797e-20</value>
+      <value>6.21245433333e-22</value>
+      <value>-2.12219325097e-21</value>
+      <value>-2.35461799216e-22</value>
+      <value>2.26518223565e-21</value>
+      <value>7.96118638110e-22</value>
+      <value>5.18051454455e-22</value>
+      <value>-4.01487854682e-21</value>
+      <value>-1.50729141697e-21</value>
+      <value>-1.59272388149e-21</value>
+      <value>-3.73218374267e-22</value>
+      <value>-1.91801774992e-21</value>
+      <value>1.15588902017e-21</value>
+      <value>-1.15595517801e-21</value>
+      <value>-6.29775860873e-22</value>
+      <value>-1.59746996636e-21</value>
+      <value>-1.04311104136e-21</value>
+      <value>-1.55408811366e-21</value>
+      <value>2.64225407008e-21</value>
+      <value>4.65128432380e-22</value>
+      <value>-1.93285340710e-21</value>
+      <value>5.51539879439e-22</value>
+      <value>2.83013490453e-22</value>
+      <value>-1.19199180477e-21</value>
+      <value>1.65869083237e-21</value>
+      <value>-2.14091049859e-23</value>
+      <value>5.53048063276e-21</value>
+      <value>-2.50142729043e-21</value>
+      <value>1.18329482973e-21</value>
+      <value>-4.78624931662e-22</value>
+      <value>-1.23352456807e-21</value>
+      <value>-8.59403201909e-22</value>
+      <value>-9.42087592015e-22</value>
+      <value>-9.14603467875e-22</value>
+      <value>1.69274107624e-21</value>
+      <value>8.00678688662e-22</value>
+      <value>1.18107266933e-21</value>
+      <value>6.78618939223e-22</value>
+      <value>2.22243618173e-22</value>
+      <value>2.20242021849e-22</value>
+      <value>-6.01764875769e-22</value>
+      <value>5.02976293280e-22</value>
+      <value>-2.13199743638e-24</value>
+      <value>2.42399216575e-22</value>
+      <value>1.10633700805e-22</value>
+      <value>2.38576479191e-22</value>
+      <value>-4.25132055300e-23</value>
+      <value>5.80214517538e-22</value>
+      <value>-1.47450733488e-22</value>
+      <value>-1.07950856190e-22</value>
+      <value>1.61117583042e-22</value>
+      <value>-3.21027750556e-22</value>
+      <value>4.28460412217e-22</value>
+      <value>-3.10830221860e-22</value>
+      <value>1.53634243383e-20</value>
+      <value>-5.02594196304e-20</value>
+      <value>5.65469497470e-20</value>
+      <value>-5.34616558682e-20</value>
+      <value>2.48283584955e-20</value>
+      <value>4.55361683233e-20</value>
+      <value>1.47350216469e-20</value>
+      <value>-6.20190183747e-21</value>
+      <value>-2.48573880729e-21</value>
+      <value>-1.25799261569e-21</value>
+      <value>3.17236912421e-21</value>
+      <value>6.77226488780e-21</value>
+      <value>-1.32132017789e-20</value>
+      <value>3.25655339302e-21</value>
+      <value>-8.08295228739e-21</value>
+      <value>5.57025237011e-21</value>
+      <value>-2.43836330419e-20</value>
+      <value>-1.40143961712e-23</value>
+      <value>9.72510874308e-22</value>
+      <value>1.97433346827e-20</value>
+      <value>3.61809020668e-21</value>
+      <value>-2.02379947786e-20</value>
+      <value>-1.04959355949e-21</value>
+      <value>-1.43130983673e-21</value>
+      <value>-9.76999054934e-21</value>
+      <value>4.52471785251e-21</value>
+      <value>-5.73962739110e-22</value>
+      <value>5.32190233084e-20</value>
+      <value>-2.50361681686e-20</value>
+      <value>1.47448596702e-20</value>
+      <value>-1.20356138264e-21</value>
+      <value>-1.90426010933e-20</value>
+      <value>-1.21140519904e-20</value>
+      <value>-5.52316393494e-21</value>
+      <value>-4.78144308017e-21</value>
+      <value>1.95872099976e-20</value>
+      <value>4.38068797804e-21</value>
+      <value>1.34802650049e-21</value>
+      <value>4.60655364314e-22</value>
+      <value>-6.15583251978e-21</value>
+      <value>-1.22036423595e-21</value>
+      <value>-6.93517921457e-21</value>
+      <value>4.99428536080e-21</value>
+      <value>3.29261073955e-21</value>
+      <value>-1.02090410120e-22</value>
+      <value>-1.31888739945e-21</value>
+      <value>1.85659650908e-21</value>
+      <value>2.16070107025e-21</value>
+      <value>2.99309978290e-21</value>
+      <value>4.05354415916e-22</value>
+      <value>-2.13463618788e-21</value>
+      <value>1.05957565959e-21</value>
+      <value>-8.76883590592e-22</value>
+      <value>2.95195703961e-22</value>
+      <value>-5.31353715421e-24</value>
+      <value>2.25220136004e-20</value>
+      <value>-1.64382251128e-20</value>
+      <value>-8.80090385645e-21</value>
+      <value>2.04351103101e-20</value>
+      <value>-1.17168350066e-20</value>
+      <value>5.50543446350e-21</value>
+      <value>-5.39177056660e-21</value>
+      <value>1.45173503711e-21</value>
+      <value>-4.95774520632e-21</value>
+      <value>3.61834249079e-21</value>
+      <value>5.95306174652e-22</value>
+      <value>-1.56293435834e-22</value>
+      <value>-5.58779164545e-21</value>
+      <value>7.31088214491e-22</value>
+      <value>1.45111484889e-21</value>
+      <value>4.58007558036e-21</value>
+      <value>-7.16588668489e-21</value>
+      <value>-3.20508868556e-21</value>
+      <value>5.20464666873e-22</value>
+      <value>8.03094478750e-22</value>
+      <value>-1.42697791324e-21</value>
+      <value>2.58957359540e-22</value>
+      <value>6.95382517595e-22</value>
+      <value>-1.84426993367e-21</value>
+      <value>-1.15764958780e-21</value>
+      <value>-1.49967688412e-21</value>
+      <value>-2.47576683687e-21</value>
+      <value>-8.33402180338e-22</value>
+      <value>6.63693220561e-22</value>
+      <value>-8.42709172044e-23</value>
+      <value>9.99597701724e-23</value>
+      <value>-3.37207170739e-22</value>
+      <value>4.73906125007e-22</value>
+      <value>-8.92808404250e-22</value>
+      <value>4.35388708773e-22</value>
+      <value>6.25070473935e-22</value>
+      <value>-8.32073507532e-23</value>
+      <value>-7.82068738481e-23</value>
+      <value>4.97941605347e-22</value>
+      <value>-7.41089548052e-24</value>
+      <value>-2.20117784801e-22</value>
+      <value>-3.28529387715e-22</value>
+      <value>3.11236700405e-22</value>
+      <value>-1.51610974637e-22</value>
+      <value>-3.44944042949e-24</value>
+      <value>1.27044194260e-21</value>
+      <value>-2.21049501716e-22</value>
+      <value>1.28883828359e-22</value>
+      <value>4.91793179642e-22</value>
+      <value>-1.61567561893e-22</value>
+      <value>2.61419701083e-22</value>
+      <value>4.86336360451e-23</value>
+      <value>-7.75064927271e-22</value>
+      <value>8.51459507438e-23</value>
+      <value>-2.65682981937e-22</value>
     </bpSampledBases>
     <rpSampledBases dimension="55">
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>0.00000</value>
-      <value>3.14369e-22</value>
-      <value>-5.47120e-22</value>
-      <value>-4.19887e-22</value>
-      <value>-3.86842e-22</value>
-      <value>-1.16978e-22</value>
-      <value>7.59626e-22</value>
-      <value>1.40619e-22</value>
-      <value>-8.67109e-23</value>
-      <value>2.00996e-22</value>
-      <value>-2.33988e-22</value>
-      <value>9.30875e-23</value>
-      <value>-1.26047e-22</value>
-      <value>-4.74135e-22</value>
-      <value>-2.51746e-22</value>
-      <value>-3.36476e-22</value>
-      <value>-1.46993e-22</value>
-      <value>2.33228e-22</value>
-      <value>3.12006e-22</value>
-      <value>2.14795e-22</value>
-      <value>-2.16999e-22</value>
-      <value>6.44248e-22</value>
-      <value>6.95423e-23</value>
-      <value>3.93629e-22</value>
-      <value>-1.73816e-24</value>
-      <value>5.12176e-22</value>
-      <value>1.65126e-22</value>
-      <value>5.95513e-22</value>
-      <value>7.13148e-22</value>
-      <value>-7.56218e-22</value>
-      <value>2.75540e-22</value>
-      <value>7.33507e-22</value>
-      <value>-5.01103e-22</value>
-      <value>4.23949e-22</value>
-      <value>-3.98454e-22</value>
-      <value>-2.55623e-22</value>
-      <value>-6.05286e-22</value>
-      <value>2.13449e-22</value>
-      <value>-3.38825e-22</value>
-      <value>-3.29538e-22</value>
-      <value>3.56279e-22</value>
-      <value>-6.74355e-23</value>
-      <value>3.50746e-22</value>
-      <value>1.18038e-22</value>
-      <value>-8.97555e-23</value>
-      <value>4.63873e-22</value>
-      <value>-4.81110e-22</value>
-      <value>1.58477e-22</value>
-      <value>1.66514e-22</value>
-      <value>4.39348e-22</value>
-      <value>6.10177e-22</value>
-      <value>7.72443e-23</value>
-      <value>-1.16950e-24</value>
-      <value>-8.73304e-23</value>
-      <value>-1.26296e-22</value>
-      <value>1.00081e-23</value>
-      <value>9.42237e-21</value>
-      <value>-1.12664e-20</value>
-      <value>-4.67037e-21</value>
-      <value>-8.43886e-22</value>
-      <value>2.66285e-22</value>
-      <value>1.88807e-21</value>
-      <value>1.13031e-21</value>
-      <value>1.40447e-21</value>
-      <value>-8.51067e-22</value>
-      <value>-2.95021e-22</value>
-      <value>-1.22538e-21</value>
-      <value>-3.21582e-21</value>
-      <value>-2.49199e-21</value>
-      <value>1.78139e-21</value>
-      <value>-3.03633e-21</value>
-      <value>6.51473e-24</value>
-      <value>9.71241e-22</value>
-      <value>1.04698e-21</value>
-      <value>2.99852e-22</value>
-      <value>-3.90245e-22</value>
-      <value>2.30208e-21</value>
-      <value>1.31837e-22</value>
-      <value>1.48903e-21</value>
-      <value>-9.27652e-23</value>
-      <value>1.99995e-21</value>
-      <value>1.19278e-21</value>
-      <value>4.04587e-21</value>
-      <value>4.81932e-21</value>
-      <value>-3.35258e-21</value>
-      <value>7.70216e-22</value>
-      <value>3.36733e-21</value>
-      <value>-2.38205e-21</value>
-      <value>7.53345e-22</value>
-      <value>-9.41171e-22</value>
-      <value>-2.26761e-21</value>
-      <value>-2.94701e-21</value>
-      <value>1.46090e-21</value>
-      <value>-7.89534e-22</value>
-      <value>-1.62766e-21</value>
-      <value>1.91441e-21</value>
-      <value>-4.54335e-22</value>
-      <value>1.94887e-21</value>
-      <value>1.42944e-21</value>
-      <value>-2.70704e-22</value>
-      <value>1.97434e-21</value>
-      <value>-2.65398e-21</value>
-      <value>8.50019e-22</value>
-      <value>1.55895e-21</value>
-      <value>1.62186e-21</value>
-      <value>2.87742e-21</value>
-      <value>1.76146e-23</value>
-      <value>-3.20279e-22</value>
-      <value>-3.40455e-22</value>
-      <value>-4.32280e-22</value>
-      <value>-1.78945e-23</value>
-      <value>1.69496e-20</value>
-      <value>2.38434e-21</value>
-      <value>1.24292e-20</value>
-      <value>-1.69054e-21</value>
-      <value>-8.53085e-22</value>
-      <value>2.01852e-21</value>
-      <value>-2.93425e-22</value>
-      <value>-2.31629e-21</value>
-      <value>-2.38326e-21</value>
-      <value>2.02763e-21</value>
-      <value>1.74218e-22</value>
-      <value>-1.08238e-22</value>
-      <value>6.36463e-22</value>
-      <value>-8.21363e-22</value>
-      <value>7.75791e-22</value>
-      <value>2.63959e-21</value>
-      <value>1.54524e-22</value>
-      <value>-1.15186e-21</value>
-      <value>1.15972e-21</value>
-      <value>8.60653e-22</value>
-      <value>6.78861e-22</value>
-      <value>4.91576e-22</value>
-      <value>2.04997e-22</value>
-      <value>2.40297e-22</value>
-      <value>-1.43902e-22</value>
-      <value>-3.04339e-23</value>
-      <value>-2.28407e-22</value>
-      <value>1.50212e-22</value>
-      <value>1.72164e-22</value>
-      <value>4.86996e-23</value>
-      <value>7.24992e-23</value>
-      <value>-5.53285e-23</value>
-      <value>4.65379e-23</value>
-      <value>1.08381e-22</value>
-      <value>9.59738e-23</value>
-      <value>-2.31756e-22</value>
-      <value>-1.75266e-22</value>
-      <value>1.62203e-22</value>
-      <value>-5.40588e-23</value>
-      <value>-1.27118e-22</value>
-      <value>-2.10288e-23</value>
-      <value>-6.63315e-23</value>
-      <value>-6.51306e-23</value>
-      <value>-7.09948e-23</value>
-      <value>2.30774e-23</value>
-      <value>-4.41078e-23</value>
-      <value>-1.90309e-23</value>
-      <value>5.39029e-23</value>
-      <value>-1.05716e-23</value>
-      <value>-4.33562e-24</value>
-      <value>-2.79900e-23</value>
-      <value>-1.08635e-22</value>
-      <value>-3.09200e-22</value>
-      <value>6.47580e-24</value>
-      <value>1.36726e-23</value>
+      <value>3.67432246688e-21</value>
+      <value>-4.43542687477e-21</value>
+      <value>-1.91756739715e-21</value>
+      <value>-4.09397411769e-22</value>
+      <value>1.11987689805e-22</value>
+      <value>9.86575444841e-22</value>
+      <value>4.24251462978e-22</value>
+      <value>5.81403725134e-22</value>
+      <value>-3.57845487389e-22</value>
+      <value>-2.27277012971e-22</value>
+      <value>-4.25841611663e-22</value>
+      <value>-1.43233303299e-21</value>
+      <value>-1.03321910380e-21</value>
+      <value>7.05933046789e-22</value>
+      <value>-1.25964440139e-21</value>
+      <value>-4.13098384521e-23</value>
+      <value>4.56601089026e-22</value>
+      <value>4.42393620309e-22</value>
+      <value>1.14216542441e-22</value>
+      <value>-2.08321421701e-22</value>
+      <value>9.70830227695e-22</value>
+      <value>5.44838816437e-23</value>
+      <value>6.44032676468e-22</value>
+      <value>-3.61129225650e-23</value>
+      <value>8.95334675394e-22</value>
+      <value>5.25331143799e-22</value>
+      <value>1.65648210818e-21</value>
+      <value>1.97021809087e-21</value>
+      <value>-1.42242321307e-21</value>
+      <value>3.71977816861e-22</value>
+      <value>1.43723181272e-21</value>
+      <value>-1.01993768623e-21</value>
+      <value>3.85087608756e-22</value>
+      <value>-4.35865081422e-22</value>
+      <value>-9.65422627209e-22</value>
+      <value>-1.27427430996e-21</value>
+      <value>6.60753693558e-22</value>
+      <value>-3.16793102700e-22</value>
+      <value>-6.73274985196e-22</value>
+      <value>8.01664309780e-22</value>
+      <value>-1.88809784730e-22</value>
+      <value>8.15268247596e-22</value>
+      <value>6.00001808862e-22</value>
+      <value>-1.05269057386e-22</value>
+      <value>8.30522278302e-22</value>
+      <value>-1.10156570984e-21</value>
+      <value>3.44923328980e-22</value>
+      <value>6.27596116760e-22</value>
+      <value>7.06375952267e-22</value>
+      <value>1.22355160571e-21</value>
+      <value>-5.63540561948e-26</value>
+      <value>-1.50838675139e-22</value>
+      <value>-1.70535774588e-22</value>
+      <value>-1.89138827657e-22</value>
+      <value>-6.66856672293e-25</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>0.00000000000</value>
+      <value>2.51964000625e-22</value>
+      <value>-4.41271143752e-22</value>
+      <value>-3.17450301636e-22</value>
+      <value>-3.79935442986e-22</value>
+      <value>-2.94560870454e-23</value>
+      <value>7.61093833906e-22</value>
+      <value>2.67005983059e-22</value>
+      <value>8.94466277420e-23</value>
+      <value>1.07230304317e-22</value>
+      <value>-1.70537024721e-22</value>
+      <value>7.03952179810e-23</value>
+      <value>-2.92765577085e-22</value>
+      <value>-3.44232163850e-22</value>
+      <value>-6.89054307597e-23</value>
+      <value>-4.39296921171e-22</value>
+      <value>-1.09275061649e-22</value>
+      <value>1.28080960259e-22</value>
+      <value>2.04331895058e-22</value>
+      <value>5.38826847471e-23</value>
+      <value>-1.18828927377e-22</value>
+      <value>3.45447402616e-22</value>
+      <value>7.36226727882e-23</value>
+      <value>3.00333621476e-22</value>
+      <value>6.00775227083e-23</value>
+      <value>3.78936742856e-22</value>
+      <value>1.28253549469e-22</value>
+      <value>3.90746113547e-22</value>
+      <value>5.48039221136e-22</value>
+      <value>-5.51327102679e-22</value>
+      <value>1.61522684707e-22</value>
+      <value>5.45365864460e-22</value>
+      <value>-3.66623964511e-22</value>
+      <value>2.02080888740e-22</value>
+      <value>-1.99129428048e-22</value>
+      <value>-2.69379096461e-22</value>
+      <value>-4.29256179478e-22</value>
+      <value>1.91145956718e-22</value>
+      <value>-1.77634425344e-22</value>
+      <value>-2.29187749830e-22</value>
+      <value>2.57407422101e-22</value>
+      <value>-5.20827711558e-23</value>
+      <value>2.67215816745e-22</value>
+      <value>1.35607218288e-22</value>
+      <value>-5.25532305610e-23</value>
+      <value>3.12122357966e-22</value>
+      <value>-3.52868475513e-22</value>
+      <value>1.07111367423e-22</value>
+      <value>1.27674467464e-22</value>
+      <value>3.16218743222e-22</value>
+      <value>4.56673282299e-22</value>
+      <value>6.21153659748e-23</value>
+      <value>-5.85379484689e-24</value>
+      <value>-6.24092179989e-23</value>
+      <value>-9.78903515603e-23</value>
+      <value>7.31391727458e-24</value>
     </rpSampledBases>
   </XpSampling>
   <XpMerge>
     <sampleMeanWavelengths>
-      <value>364.398</value>
-      <value>438.798</value>
-      <value>551.607</value>
-      <value>652.354</value>
-      <value>798.973</value>
+      <value>542.695</value>
+      <value>419.775</value>
+      <value>531.453</value>
     </sampleMeanWavelengths>
     <bpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
-      <value>1.00000</value>
     </bpWeights>
     <rpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
-      <value>1.00000</value>
     </rpWeights>
   </XpMerge>
   <fluxBias>
-    <value>2.44819e-19</value>
-    <value>4.62320e-20</value>
-    <value>1.81103e-20</value>
-    <value>2.15027e-20</value>
-    <value>1.73864e-20</value>
+    <value>0.00000</value>
+    <value>0.00000</value>
+    <value>0.00000</value>
   </fluxBias>
   <zeropoints>
-    <value>-25.8489</value>
-    <value>-25.4710</value>
-    <value>-26.0861</value>
-    <value>-26.6268</value>
-    <value>-27.3212</value>
+    <value>-26.0414</value>
+    <value>-25.4434</value>
+    <value>-26.0002</value>
   </zeropoints>
 </config>
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Stromgren_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_GaiaNominal_v375wiv142r.xml`

 * *Files 25% similar despite different names*

#### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/filters/XpFilter_Stromgren_v375wiv142r.xml` & `gaiaxpy-2.1.1/src/gaiaxpy/config/filters/XpFilter_GaiaNominal_v375wiv142r.xml`

```diff
@@ -1,488 +1,372 @@
 <?xml version="1.0" encoding="utf-8"?>
 <config>
   <solutionId>4545469030156206114</solutionId>
-  <bands n="4">
-    <item>u</item>
-    <item>v</item>
-    <item>b</item>
-    <item>y</item>
+  <bands n="3">
+    <item>G</item>
+    <item>BP</item>
+    <item>RP</item>
   </bands>
   <XpSampling>
     <bpSampledBases dimension="55">
-      <value>9.33782382157e-21</value>
-      <value>-3.58692954997e-20</value>
-      <value>5.70227509367e-20</value>
-      <value>-7.87210689822e-20</value>
-      <value>9.74868410085e-20</value>
-      <value>1.73176761795e-19</value>
-      <value>-1.06341252166e-19</value>
-      <value>1.13335587192e-19</value>
-      <value>-4.88586237188e-19</value>
-      <value>1.60690498832e-20</value>
-      <value>-1.49794044220e-19</value>
-      <value>3.66648565194e-20</value>
-      <value>1.27148000704e-19</value>
-      <value>3.06913784172e-20</value>
-      <value>4.72507165876e-21</value>
-      <value>-1.51273220936e-20</value>
-      <value>1.79908316549e-19</value>
-      <value>-9.72163625636e-21</value>
-      <value>-4.73313907203e-20</value>
-      <value>-1.83528078563e-19</value>
-      <value>6.87200577886e-20</value>
-      <value>-2.42844007965e-20</value>
-      <value>-3.28111799064e-19</value>
-      <value>1.44098373023e-19</value>
-      <value>1.64352830658e-19</value>
-      <value>-3.20769953569e-19</value>
-      <value>-3.22229384266e-19</value>
-      <value>1.14812132065e-19</value>
-      <value>1.98921779431e-19</value>
-      <value>-6.05819374946e-19</value>
-      <value>-5.02965737322e-20</value>
-      <value>2.32921756004e-19</value>
-      <value>-2.79979707064e-19</value>
-      <value>2.02243806551e-19</value>
-      <value>3.40676809468e-19</value>
-      <value>-7.76576196489e-20</value>
-      <value>-5.11999364313e-19</value>
-      <value>1.77106655328e-19</value>
-      <value>5.85149534915e-19</value>
-      <value>-2.09266955061e-19</value>
-      <value>-1.02391872364e-18</value>
-      <value>3.03837586742e-19</value>
-      <value>-2.99165164727e-19</value>
-      <value>4.24636436689e-19</value>
-      <value>-2.44980408325e-19</value>
-      <value>-2.97806069457e-19</value>
-      <value>-2.65886236223e-19</value>
-      <value>6.77871756590e-19</value>
-      <value>-3.09698116673e-19</value>
-      <value>1.78560064988e-19</value>
-      <value>5.28617202558e-19</value>
-      <value>6.36116143792e-20</value>
-      <value>4.87077347512e-19</value>
-      <value>-6.97395422793e-20</value>
-      <value>5.59108077511e-20</value>
-      <value>1.55660857131e-20</value>
-      <value>-5.61665402917e-20</value>
-      <value>7.50348475099e-20</value>
-      <value>-5.96331699093e-20</value>
-      <value>2.63751230726e-21</value>
-      <value>4.34983904371e-20</value>
-      <value>5.17182906784e-21</value>
-      <value>-1.32842341805e-20</value>
-      <value>2.20854427518e-20</value>
-      <value>2.53143903452e-20</value>
-      <value>1.09612543897e-20</value>
-      <value>-1.96930703983e-20</value>
-      <value>-1.17191761936e-20</value>
-      <value>-2.86403777930e-20</value>
-      <value>3.53980462192e-20</value>
-      <value>5.28064175006e-20</value>
-      <value>-3.60902047429e-20</value>
-      <value>-2.50637840995e-20</value>
-      <value>-3.72268864852e-20</value>
-      <value>-8.98682999555e-20</value>
-      <value>-1.28515878107e-19</value>
-      <value>2.30676121424e-19</value>
-      <value>-2.75447652492e-20</value>
-      <value>1.22306493404e-19</value>
-      <value>-6.29755945442e-21</value>
-      <value>7.34019240128e-21</value>
-      <value>6.91986155765e-20</value>
-      <value>1.21143238872e-20</value>
-      <value>3.01648977124e-20</value>
-      <value>2.96892796344e-20</value>
-      <value>2.07841567396e-20</value>
-      <value>2.04586132094e-20</value>
-      <value>-1.41394450664e-20</value>
-      <value>4.42708197378e-20</value>
-      <value>1.78552364949e-20</value>
-      <value>3.06037861286e-20</value>
-      <value>3.96064179934e-20</value>
-      <value>-6.48734195448e-20</value>
-      <value>-8.59542515223e-21</value>
-      <value>1.25233921311e-20</value>
-      <value>6.61636785040e-21</value>
-      <value>6.30197680030e-20</value>
-      <value>-4.15883550675e-20</value>
-      <value>-5.28618711743e-20</value>
-      <value>3.79939937440e-20</value>
-      <value>-6.96762732377e-20</value>
-      <value>-4.86072804073e-20</value>
-      <value>4.62065407437e-20</value>
-      <value>-9.56976155332e-20</value>
-      <value>-3.23011064162e-22</value>
-      <value>-1.23794058411e-19</value>
-      <value>-7.14668027970e-21</value>
-      <value>1.12912168251e-19</value>
-      <value>2.66447430624e-20</value>
-      <value>3.99020008761e-20</value>
-      <value>2.13138380531e-20</value>
-      <value>-4.13264375620e-20</value>
-      <value>-6.33255302372e-21</value>
-      <value>-7.28871305104e-21</value>
-      <value>3.73030881568e-20</value>
-      <value>-8.52441123432e-20</value>
-      <value>2.18465479714e-21</value>
-      <value>7.82471844070e-21</value>
-      <value>-1.12795939001e-20</value>
-      <value>-1.08985163118e-20</value>
-      <value>-8.48497330066e-21</value>
-      <value>5.14692569020e-21</value>
-      <value>6.91420313126e-21</value>
-      <value>-7.08355929668e-21</value>
-      <value>-1.22081712610e-20</value>
-      <value>-1.82198104468e-20</value>
-      <value>1.71302255008e-20</value>
-      <value>2.42568973473e-20</value>
-      <value>-8.13746560281e-20</value>
-      <value>2.15245811039e-20</value>
-      <value>-3.60096164558e-20</value>
-      <value>-3.62792024818e-20</value>
-      <value>9.11191755429e-20</value>
-      <value>7.44842408584e-20</value>
-      <value>4.89677308711e-20</value>
-      <value>-1.16751689338e-20</value>
-      <value>3.59243282661e-21</value>
-      <value>-2.46052399233e-20</value>
-      <value>-4.05085406723e-20</value>
-      <value>-4.96383242908e-22</value>
-      <value>-2.62555863026e-20</value>
-      <value>1.73847872134e-20</value>
-      <value>-1.14343012949e-20</value>
-      <value>3.48560633574e-20</value>
-      <value>8.57895110311e-21</value>
-      <value>-1.93240717747e-21</value>
-      <value>4.36692092755e-21</value>
-      <value>9.42760304624e-21</value>
-      <value>1.96210841787e-20</value>
-      <value>5.56908628161e-21</value>
-      <value>-7.25922209714e-22</value>
-      <value>1.78920987270e-20</value>
-      <value>2.01253243616e-20</value>
-      <value>1.89559677952e-20</value>
-      <value>-3.02256603598e-20</value>
-      <value>1.52446759829e-21</value>
-      <value>3.82389346072e-20</value>
-      <value>-1.97157333356e-20</value>
-      <value>-2.78783596915e-20</value>
-      <value>-2.43801235474e-20</value>
-      <value>-2.97568755039e-20</value>
-      <value>-1.03728574618e-20</value>
-      <value>6.95206714670e-21</value>
-      <value>7.37639919168e-21</value>
-      <value>-1.17974630296e-20</value>
-      <value>2.44126120428e-20</value>
-      <value>-8.01145971227e-21</value>
-      <value>-1.72432037044e-20</value>
-      <value>3.12747415393e-20</value>
-      <value>2.77823791055e-20</value>
-      <value>2.43402401915e-20</value>
-      <value>2.91613356603e-20</value>
-      <value>-6.34043739002e-21</value>
-      <value>1.09013708285e-21</value>
-      <value>-5.45957925186e-20</value>
-      <value>8.70503042021e-21</value>
-      <value>6.09505598087e-20</value>
-      <value>4.82001351307e-20</value>
-      <value>-2.26785237438e-20</value>
-      <value>8.44547722036e-22</value>
-      <value>1.07510627999e-19</value>
-      <value>6.21648576799e-20</value>
-      <value>-6.95887279033e-20</value>
-      <value>6.04229511140e-22</value>
-      <value>5.41938757231e-20</value>
-      <value>-1.76286013057e-20</value>
-      <value>-4.95783808304e-21</value>
-      <value>-1.59558912305e-20</value>
-      <value>6.55170507289e-21</value>
-      <value>-2.33035971624e-20</value>
-      <value>5.22049662574e-20</value>
-      <value>-1.93682752078e-20</value>
-      <value>2.01208081637e-21</value>
-      <value>-8.16927975593e-22</value>
-      <value>-1.20054653877e-20</value>
-      <value>-2.90583375030e-20</value>
-      <value>1.87114158276e-20</value>
-      <value>5.83410451552e-21</value>
-      <value>1.42434226059e-20</value>
-      <value>-1.43651507647e-20</value>
-      <value>-1.87050005696e-20</value>
-      <value>7.86560982311e-21</value>
-      <value>1.32180354929e-21</value>
-      <value>8.74930751782e-21</value>
-      <value>1.15322170908e-20</value>
-      <value>4.01858919663e-21</value>
-      <value>1.41922854545e-20</value>
-      <value>1.45458608641e-20</value>
-      <value>-2.68955023266e-21</value>
-      <value>2.17922036443e-20</value>
-      <value>6.43267725162e-21</value>
-      <value>-2.02676704769e-20</value>
-      <value>-1.00661551810e-20</value>
-      <value>3.01383979541e-20</value>
-      <value>-3.68198263960e-21</value>
-      <value>2.42023934987e-20</value>
-      <value>1.74558094087e-21</value>
-      <value>-4.02700610437e-20</value>
-      <value>1.16169129358e-20</value>
-      <value>-2.30727201105e-20</value>
+      <value>9.60942e-21</value>
+      <value>-6.08637e-21</value>
+      <value>-6.20056e-22</value>
+      <value>-2.68738e-21</value>
+      <value>-8.39341e-22</value>
+      <value>2.06188e-21</value>
+      <value>9.46092e-22</value>
+      <value>1.72235e-22</value>
+      <value>-2.43145e-21</value>
+      <value>-1.60390e-21</value>
+      <value>-1.41804e-21</value>
+      <value>-9.51477e-22</value>
+      <value>-5.74201e-22</value>
+      <value>9.00143e-22</value>
+      <value>-5.38916e-22</value>
+      <value>-4.27373e-22</value>
+      <value>-2.07889e-22</value>
+      <value>-1.26161e-21</value>
+      <value>-5.98022e-22</value>
+      <value>5.08640e-22</value>
+      <value>3.71671e-22</value>
+      <value>-2.82670e-22</value>
+      <value>-5.27492e-22</value>
+      <value>5.26665e-22</value>
+      <value>-4.57893e-22</value>
+      <value>5.25838e-22</value>
+      <value>-4.08715e-22</value>
+      <value>6.22107e-22</value>
+      <value>-2.46669e-23</value>
+      <value>-6.67905e-22</value>
+      <value>-7.78334e-22</value>
+      <value>4.01163e-22</value>
+      <value>-2.92394e-22</value>
+      <value>-1.15980e-23</value>
+      <value>4.25194e-22</value>
+      <value>2.25376e-22</value>
+      <value>-2.49335e-22</value>
+      <value>4.72327e-22</value>
+      <value>5.04812e-22</value>
+      <value>7.63337e-24</value>
+      <value>-1.00531e-21</value>
+      <value>9.61789e-22</value>
+      <value>1.02792e-22</value>
+      <value>3.58208e-22</value>
+      <value>-2.49091e-22</value>
+      <value>1.04013e-22</value>
+      <value>-1.39863e-22</value>
+      <value>3.20213e-22</value>
+      <value>-9.50201e-24</value>
+      <value>-1.23695e-22</value>
+      <value>4.29793e-22</value>
+      <value>8.41332e-23</value>
+      <value>2.46007e-22</value>
+      <value>2.37860e-22</value>
+      <value>-2.55135e-22</value>
+      <value>1.92938e-20</value>
+      <value>-1.59248e-20</value>
+      <value>3.07712e-21</value>
+      <value>-8.37355e-21</value>
+      <value>1.32601e-21</value>
+      <value>8.01135e-21</value>
+      <value>5.42585e-22</value>
+      <value>2.06523e-21</value>
+      <value>-1.23409e-20</value>
+      <value>-2.07190e-21</value>
+      <value>-4.53400e-21</value>
+      <value>-7.34692e-22</value>
+      <value>-6.91999e-22</value>
+      <value>2.65482e-21</value>
+      <value>-1.32415e-21</value>
+      <value>-1.06864e-21</value>
+      <value>9.50762e-22</value>
+      <value>-1.63916e-21</value>
+      <value>-1.44929e-21</value>
+      <value>3.84864e-22</value>
+      <value>1.22211e-21</value>
+      <value>-8.37148e-22</value>
+      <value>-1.51844e-21</value>
+      <value>9.43626e-22</value>
+      <value>-4.94281e-22</value>
+      <value>1.98331e-22</value>
+      <value>-2.19996e-21</value>
+      <value>2.61090e-21</value>
+      <value>2.25412e-22</value>
+      <value>-2.95907e-21</value>
+      <value>-1.57978e-21</value>
+      <value>9.57003e-22</value>
+      <value>-2.50497e-21</value>
+      <value>8.47606e-22</value>
+      <value>1.61637e-21</value>
+      <value>7.96782e-22</value>
+      <value>-1.15866e-21</value>
+      <value>9.32407e-22</value>
+      <value>1.29687e-21</value>
+      <value>-3.02789e-21</value>
+      <value>-7.30435e-21</value>
+      <value>3.76061e-21</value>
+      <value>-2.63958e-22</value>
+      <value>2.32168e-21</value>
+      <value>-1.67236e-21</value>
+      <value>-6.62034e-22</value>
+      <value>-1.85876e-21</value>
+      <value>4.38431e-21</value>
+      <value>3.93417e-22</value>
+      <value>-2.37294e-21</value>
+      <value>3.77776e-21</value>
+      <value>5.83383e-22</value>
+      <value>2.84811e-22</value>
+      <value>-7.13608e-22</value>
+      <value>-1.07828e-21</value>
+      <value>6.79549e-22</value>
+      <value>7.99799e-22</value>
+      <value>7.88005e-22</value>
+      <value>-1.25252e-22</value>
+      <value>-1.15309e-21</value>
+      <value>-2.82025e-22</value>
+      <value>1.31128e-21</value>
+      <value>4.71319e-22</value>
+      <value>-8.60549e-22</value>
+      <value>-1.51520e-21</value>
+      <value>1.26419e-21</value>
+      <value>-1.15041e-21</value>
+      <value>8.03289e-22</value>
+      <value>1.14447e-21</value>
+      <value>-6.87479e-22</value>
+      <value>1.09419e-21</value>
+      <value>5.30685e-22</value>
+      <value>-5.52457e-22</value>
+      <value>-5.60882e-22</value>
+      <value>3.66299e-22</value>
+      <value>-7.77837e-22</value>
+      <value>-4.69381e-22</value>
+      <value>-9.10608e-22</value>
+      <value>-1.55176e-23</value>
+      <value>5.48452e-22</value>
+      <value>3.44800e-22</value>
+      <value>3.64405e-22</value>
+      <value>-4.49848e-22</value>
+      <value>-7.59975e-22</value>
+      <value>-3.98761e-24</value>
+      <value>-1.90959e-22</value>
+      <value>5.00073e-23</value>
+      <value>-1.88216e-22</value>
+      <value>4.01088e-22</value>
+      <value>8.26045e-23</value>
+      <value>2.24885e-22</value>
+      <value>-5.47578e-23</value>
+      <value>2.01593e-22</value>
+      <value>3.01996e-22</value>
+      <value>3.19639e-22</value>
+      <value>-1.49550e-22</value>
+      <value>2.42323e-22</value>
+      <value>8.98679e-22</value>
+      <value>3.85769e-22</value>
+      <value>-7.65607e-22</value>
+      <value>5.18282e-22</value>
+      <value>3.07144e-22</value>
+      <value>-1.29387e-22</value>
+      <value>-9.27958e-22</value>
+      <value>-2.36637e-22</value>
+      <value>-1.04372e-21</value>
+      <value>-8.38214e-23</value>
+      <value>8.80988e-22</value>
+      <value>2.87654e-22</value>
+      <value>-7.18800e-23</value>
     </bpSampledBases>
     <rpSampledBases dimension="55">
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
-      <value>0.00000000000</value>
+      <value>9.75490e-21</value>
+      <value>-2.75925e-21</value>
+      <value>-2.21195e-21</value>
+      <value>2.32594e-22</value>
+      <value>8.22529e-22</value>
+      <value>2.59681e-22</value>
+      <value>1.56407e-21</value>
+      <value>-2.97035e-22</value>
+      <value>-1.41212e-21</value>
+      <value>3.55564e-22</value>
+      <value>3.76139e-22</value>
+      <value>-8.85750e-22</value>
+      <value>-1.56669e-21</value>
+      <value>1.20124e-21</value>
+      <value>-1.29595e-21</value>
+      <value>-1.86507e-22</value>
+      <value>2.27922e-22</value>
+      <value>-3.24986e-22</value>
+      <value>-1.68968e-22</value>
+      <value>1.36719e-22</value>
+      <value>1.39083e-21</value>
+      <value>-2.54488e-22</value>
+      <value>1.42109e-21</value>
+      <value>-8.92543e-22</value>
+      <value>1.05493e-21</value>
+      <value>9.82480e-23</value>
+      <value>1.77876e-21</value>
+      <value>1.39809e-21</value>
+      <value>-1.24462e-21</value>
+      <value>-1.99440e-22</value>
+      <value>1.27801e-21</value>
+      <value>-1.25575e-21</value>
+      <value>5.21018e-22</value>
+      <value>7.49630e-22</value>
+      <value>2.60669e-22</value>
+      <value>-1.84551e-21</value>
+      <value>2.16582e-21</value>
+      <value>-1.84070e-21</value>
+      <value>9.54674e-22</value>
+      <value>-5.31022e-22</value>
+      <value>-1.83587e-21</value>
+      <value>3.04257e-22</value>
+      <value>1.01074e-21</value>
+      <value>-3.90864e-21</value>
+      <value>1.44073e-21</value>
+      <value>-2.12627e-21</value>
+      <value>-4.31362e-21</value>
+      <value>-4.57827e-22</value>
+      <value>9.83921e-22</value>
+      <value>-2.17134e-22</value>
+      <value>-1.06936e-21</value>
+      <value>-1.13559e-21</value>
+      <value>5.46491e-21</value>
+      <value>1.25455e-21</value>
+      <value>3.28476e-21</value>
+      <value>2.05696e-21</value>
+      <value>-3.55301e-21</value>
+      <value>-2.35617e-21</value>
+      <value>-2.53255e-21</value>
+      <value>4.76291e-22</value>
+      <value>5.63199e-21</value>
+      <value>2.64218e-21</value>
+      <value>2.27148e-21</value>
+      <value>-1.69680e-22</value>
+      <value>-8.35207e-22</value>
+      <value>2.17753e-22</value>
+      <value>-3.84898e-21</value>
+      <value>-1.61041e-21</value>
+      <value>1.00186e-21</value>
+      <value>-3.74628e-21</value>
+      <value>-4.89959e-22</value>
+      <value>2.57292e-22</value>
+      <value>7.63861e-22</value>
+      <value>-5.60315e-22</value>
+      <value>-1.41863e-22</value>
+      <value>5.92947e-22</value>
+      <value>5.16460e-22</value>
+      <value>1.21605e-21</value>
+      <value>5.27320e-22</value>
+      <value>1.53258e-21</value>
+      <value>1.37306e-22</value>
+      <value>9.00770e-22</value>
+      <value>2.88401e-21</value>
+      <value>-3.55418e-21</value>
+      <value>6.27888e-22</value>
+      <value>3.86693e-21</value>
+      <value>-2.33226e-21</value>
+      <value>-1.01690e-22</value>
+      <value>2.84796e-22</value>
+      <value>-2.65834e-21</value>
+      <value>-2.05182e-21</value>
+      <value>1.71637e-21</value>
+      <value>5.95625e-22</value>
+      <value>-9.52525e-22</value>
+      <value>1.04229e-21</value>
+      <value>-3.78655e-22</value>
+      <value>1.26954e-21</value>
+      <value>1.57244e-21</value>
+      <value>1.72097e-24</value>
+      <value>4.30748e-22</value>
+      <value>-6.54556e-22</value>
+      <value>6.16532e-23</value>
+      <value>5.29187e-22</value>
+      <value>-3.13991e-22</value>
+      <value>5.62047e-22</value>
+      <value>1.22942e-22</value>
+      <value>-9.14214e-23</value>
+      <value>-1.19617e-22</value>
+      <value>1.35978e-22</value>
+      <value>1.42888e-22</value>
+      <value>1.64434e-20</value>
+      <value>5.73671e-22</value>
+      <value>-5.35310e-21</value>
+      <value>1.19312e-21</value>
+      <value>2.24442e-21</value>
+      <value>3.68823e-22</value>
+      <value>4.11078e-21</value>
+      <value>-2.10536e-21</value>
+      <value>-4.16072e-21</value>
+      <value>1.14957e-21</value>
+      <value>2.54360e-21</value>
+      <value>-1.93786e-22</value>
+      <value>-3.05781e-21</value>
+      <value>2.45581e-21</value>
+      <value>-1.61989e-21</value>
+      <value>-6.56311e-22</value>
+      <value>-2.86950e-23</value>
+      <value>-2.18066e-21</value>
+      <value>-1.04548e-21</value>
+      <value>8.27516e-22</value>
+      <value>3.15883e-21</value>
+      <value>-1.17938e-21</value>
+      <value>3.64492e-21</value>
+      <value>-3.30175e-21</value>
+      <value>1.86063e-21</value>
+      <value>-8.95604e-22</value>
+      <value>2.56886e-21</value>
+      <value>3.92480e-22</value>
+      <value>-1.36512e-21</value>
+      <value>-1.48603e-21</value>
+      <value>1.26079e-21</value>
+      <value>-2.32930e-21</value>
+      <value>1.00990e-21</value>
+      <value>3.30993e-21</value>
+      <value>3.19092e-21</value>
+      <value>-3.61119e-21</value>
+      <value>6.44433e-21</value>
+      <value>-6.03380e-21</value>
+      <value>4.54629e-21</value>
+      <value>-4.06841e-21</value>
+      <value>-6.27164e-21</value>
+      <value>-7.10173e-22</value>
+      <value>2.25363e-21</value>
+      <value>-1.38038e-20</value>
+      <value>3.74320e-21</value>
+      <value>-5.76092e-21</value>
+      <value>-1.69012e-20</value>
+      <value>-4.10974e-21</value>
+      <value>2.13480e-21</value>
+      <value>-3.49987e-21</value>
+      <value>-4.09289e-21</value>
+      <value>-2.94768e-21</value>
+      <value>2.04494e-20</value>
+      <value>4.78491e-21</value>
+      <value>1.25859e-20</value>
     </rpSampledBases>
   </XpSampling>
   <XpMerge>
     <sampleMeanWavelengths>
-      <value>347.877</value>
-      <value>410.570</value>
-      <value>469.584</value>
-      <value>550.272</value>
+      <value>639.716</value>
+      <value>522.679</value>
+      <value>784.692</value>
     </sampleMeanWavelengths>
     <bpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
     </bpWeights>
     <rpWeights>
       <value>1.00000</value>
       <value>1.00000</value>
       <value>1.00000</value>
-      <value>1.00000</value>
     </rpWeights>
   </XpMerge>
   <fluxBias>
-    <value>0.00000</value>
-    <value>0.00000</value>
-    <value>0.00000</value>
-    <value>0.00000</value>
+    <value>-26.4854</value>
+    <value>-25.9782</value>
+    <value>-27.2241</value>
   </fluxBias>
   <zeropoints>
-    <value>-26.2346</value>
-    <value>-25.3302</value>
-    <value>-25.6020</value>
-    <value>-26.1045</value>
+    <value>1.00000</value>
+    <value>1.00000</value>
+    <value>1.00000</value>
   </zeropoints>
 </config>
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/rpC03_v142r_bases.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/rpC03_v142r_bases.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/rpC03_v142r_dispersion.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/rpC03_v142r_dispersion.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/config/rpC03_v142r_response.csv` & `gaiaxpy-2.1.1/src/gaiaxpy/config/rpC03_v142r_response.csv`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/converter/converter.py` & `gaiaxpy-2.1.1/src/gaiaxpy/converter/converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 converter.py
 ====================================
 Module for the converter functionality.
 """
 
 from numbers import Number
 from pathlib import Path
+from sys import stdout
 from typing import Union, Optional
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
-from gaiaxpy.core.generic_functions import cast_output, get_spectra_type, validate_arguments, validate_pwl_sampling
+from gaiaxpy.core.generic_functions import cast_output, validate_pwl_sampling, format_sampled_output
 from gaiaxpy.core.generic_variables import pbar_colour, pbar_units, pbar_message
 from gaiaxpy.core.satellite import BANDS
 from gaiaxpy.input_reader.input_reader import InputReader
 from gaiaxpy.output.sampled_spectra_data import SampledSpectraData
 from gaiaxpy.spectrum.sampled_basis_functions import SampledBasisFunctions
 from gaiaxpy.spectrum.xp_continuous_spectrum import XpContinuousSpectrum
 from gaiaxpy.spectrum.xp_sampled_spectrum import XpSampledSpectrum
-from .config import get_config, load_config
-from ..config.paths import optimised_bases_file
+from .config import parse_config, get_bands_config
+from ..config.paths import hermite_bases_file
+from ..core.input_validator import validate_save_arguments
 
 __FUNCTION_KEY = 'converter'
 
 
 def convert(input_object: Union[list, Path, str], sampling: Optional[np.ndarray] = np.linspace(0, 60, 600),
             truncation: bool = False, with_correlation: bool = False, output_path: Union[Path, str] = '.',
             output_file: str = 'output_spectra', output_format: str = None, save_file: bool = True,
@@ -63,41 +65,39 @@
                     with_correlation=with_correlation, output_path=output_path, output_file=output_file,
                     output_format=output_format, save_file=save_file, username=username, password=password)
 
 
 def _convert(input_object: Union[list, Path, str], sampling: np.ndarray = np.linspace(0, 60, 600),
              truncation: bool = False, with_correlation: bool = False, output_path: Union[Path, str] = '.',
              output_file: str = 'output_spectra', output_format: str = None, save_file: bool = True,
-             username: str = None, password: str = None, disable_info: bool = False) -> (pd.DataFrame, np.ndarray):
+             username: str = None, password: str = None, disable_info: bool = False, config_file=hermite_bases_file) \
+        -> (pd.DataFrame, np.ndarray):
     """
     Internal method of the calibration utility. Refer to "convert".
 
     Args:
         disable_info (bool): Whether to disable the progress tracker.
 
     Returns:
         DataFrame: A list of all sampled absolute spectra.
         ndarray: The sampling used to calibrate the spectra.
 
     Raises:
         ValueError: If the sampling is out of the expected boundaries.
     """
-    # Check sampling
+    function = convert
     validate_pwl_sampling(sampling)
-    validate_arguments(convert.__defaults__[4], output_file, save_file)
-    parsed_input_data, extension = InputReader(input_object, convert, disable_info=disable_info, user=username,
-                                               password=password).read()
-    config_df = load_config(optimised_bases_file)
-    # Union of unique ids as sets
-    unique_bases_ids = get_unique_basis_ids(parsed_input_data)
-    # Get design matrices
-    design_matrices = get_design_matrices(unique_bases_ids, sampling, config_df)
+    validate_save_arguments(function.__defaults__[4], output_file, function.__defaults__[5], output_format, save_file)
+    parsed_input_data, extension = InputReader(input_object, convert, truncation=truncation, disable_info=disable_info,
+                                               user=username, password=password).read()
+    bases_config = parse_config(config_file)
+    design_matrices = get_design_matrices(sampling, bases_config)
     spectra_df, positions = _create_spectra(parsed_input_data, truncation, design_matrices,
                                             with_correlation=with_correlation, disable_info=disable_info)
-    # Save output
+    # Save output section
     output_data = SampledSpectraData(spectra_df, positions)
     output_data.data = cast_output(output_data)
     output_data.save(save_file, output_path, output_file, output_format, extension)
     return output_data.data, positions
 
 
 def _create_spectrum(row: pd.Series, truncation: bool, design_matrices: dict, band: str,
@@ -114,19 +114,18 @@
             user-defined or default).
         band (str): bp/rp band.
         with_correlation (bool): Whether correlation information should be generated.
 
     Returns:
         XpSampledSpectrum: The sampled spectrum.
     """
-    covariance_matrix = row[f'{band}_covariance_matrix']
     recommended_truncation = row[f'{band}_n_relevant_bases'] if truncation else -1
     continuous_spectrum = XpContinuousSpectrum(row['source_id'], band, row[f'{band}_coefficients'],
-                                               covariance_matrix, row[f'{band}_standard_deviation'])
-    return XpSampledSpectrum.from_continuous(continuous_spectrum, design_matrices.get(row[f'{band}_basis_function_id']),
+                                               row[f'{band}_covariance_matrix'], row[f'{band}_standard_deviation'])
+    return XpSampledSpectrum.from_continuous(continuous_spectrum, design_matrices.get(band),
                                              truncation=recommended_truncation, with_correlation=with_correlation)
 
 
 def _create_spectra(parsed_input_data: pd.DataFrame, truncation: bool, design_matrices: dict,
                     with_correlation: bool = False, disable_info=False) -> tuple:
     """
     Creates a spectra dataframe from parsed input data and given parameters.
@@ -139,47 +138,39 @@
         with_correlation (bool): Whether to include the covariance matrix in the spectra. Default is False.
 
     Returns:
         (tuple): tuple containing:
             DataFrame: The output spectra.
             ndarray: The sampling used to convert the input spectra (user-provided or default).
     """
+
     def create_xp_spectra(row, _truncation, _design_matrices, _with_correlation=False):
         """
         Creates bp and rp spectra for a single row of parsed input data.
 
         Args:
             row (pandas Series): A single row of parsed input data.
             _truncation (bool): Toggle truncation of the set of bases. The level of truncation to be applied is defined
                 by the recommended value in the input files.
             _design_matrices (dict): The design matrices for the input list of bases.
             _with_correlation (bool): Whether to include the covariance matrix in the spectra. Default is False.
 
         Returns:
             list: A list of spectra for the given row of parsed input data containing one element per band available.
         """
-        spectra_list = []
-        for band in BANDS:
-            spectrum_xp = _create_spectrum(row, _truncation, _design_matrices, band, with_correlation=_with_correlation)
-            if spectrum_xp:
-                spectra_list.append(spectrum_xp)
-        return spectra_list
+        return [_create_spectrum(row, _truncation, _design_matrices, band, with_correlation=_with_correlation)
+                for band in BANDS]
 
     parsed_input_data_dict = parsed_input_data.to_dict('records')
     spectra_series = pd.Series([create_xp_spectra(row, truncation, design_matrices, with_correlation)
                                 for row in tqdm(parsed_input_data_dict, desc=pbar_message[__FUNCTION_KEY],
                                                 unit=pbar_units[__FUNCTION_KEY], leave=False, colour=pbar_colour,
-                                                disable=disable_info)])
+                                                disable=disable_info, file=stdout)])
     spectra_series = spectra_series.explode()
-    positions = spectra_series.iloc[0].get_positions()
-    spectra_type = get_spectra_type(spectra_series.iloc[0])
-    spectra_series = spectra_series.map(lambda x: x.spectrum_to_dict())
-    spectra_df = pd.DataFrame(spectra_series.tolist())
-    spectra_df.attrs['data_type'] = spectra_type
-    return spectra_df, positions
+    return format_sampled_output(spectra_series, with_correlation=with_correlation)
 
 
 def get_unique_basis_ids(parsed_input_data: pd.DataFrame) -> set:
     """
     Get the IDs of the unique basis required to sample all spectra in the input files.
 
     Args:
@@ -195,20 +186,26 @@
         return {int(element) for element in _set if element == element}
 
     set_bp = set([basis for basis in parsed_input_data[f'{BANDS.bp}_basis_function_id'] if isinstance(basis, Number)])
     set_rp = set([basis for basis in parsed_input_data[f'{BANDS.rp}_basis_function_id'] if isinstance(basis, Number)])
     return remove_nans(set_bp).union(remove_nans(set_rp))
 
 
-def get_design_matrices(unique_bases_ids: set, sampling: np.ndarray, config_df: pd.DataFrame) -> dict:
+def get_design_matrices(sampling: np.ndarray, bases_config: pd.DataFrame) -> dict:
     """
     Get the design matrices corresponding to the input bases.
 
     Args:
-        unique_bases_ids (set): A set containing the basis function IDs for which the design matrix is required.
         sampling (ndarray): 1D array containing the sampling grid.
-        config_df (DataFrame): A DataFrame containing the configuration for all sets of basis functions.
+        bases_config (NamedTuple): An object containing the configuration for all sets of basis functions.
 
     Returns:
         dict: The design matrices for the input list of bases.
     """
-    return {_id: SampledBasisFunctions.from_config(sampling, get_config(config_df, _id)) for _id in unique_bases_ids}
+    bands_config = get_bands_config(bases_config)
+    bp_config = bands_config.bpConfig
+    rp_config = bands_config.rpConfig
+    bp_config_dict = {field: getattr(bp_config, field) for field in bp_config._fields}
+    rp_config_dict = {field: getattr(rp_config, field) for field in rp_config._fields}
+    bands_config = {key: value for key, value in zip(BANDS, [bp_config_dict, rp_config_dict])}
+    config_df = pd.DataFrame.from_dict(bands_config, orient='index')
+    return {band: SampledBasisFunctions.from_config(sampling, config_df.loc[[band]]) for band in BANDS}
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/core/config.py` & `gaiaxpy-2.1.1/src/gaiaxpy/core/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ====================================
 Module to handle the calibrator and generator configuration files.
 """
 
 from configparser import ConfigParser
 from os.path import join
 
-from gaiaxpy.config.paths import config_path, filters_path, config_ini_file
+from gaiaxpy.config.paths import filters_path, config_ini_file
 from gaiaxpy.core.satellite import BANDS
 from gaiaxpy.core.xml_utils import get_file_root, get_array_text, get_xp_merge, get_xp_sampling_matrix
 
 ADDITIONAL_SYSTEM_PREFIX = 'USER'
 
 
 def get_file_path(config_file=None):
@@ -23,15 +23,14 @@
         file_path = _config_parser['filter']['filters_dir']
     except KeyError:
         return filters_path
     return file_path
 
 
 def get_filter_version_from_config(_config_parser):
-    # TODO: return built-in version if the version section is not found.
     try:
         version = _config_parser['filter']['version']
     except KeyError:
         version = None
     return version
 
 
@@ -39,15 +38,16 @@
     _config_parser = ConfigParser()
     _config_parser.read(_config_file)
     version = get_filter_version_from_config(_config_parser)
     if version:
         file_name = _config_parser.get(label, key).replace('version', version)
         system = system.replace(f'{ADDITIONAL_SYSTEM_PREFIX}_', '')
     else:
-        file_name = _config_parser.get(label, key).format(label, key).replace('model', f'{bp_model}{rp_model}')
+        file_name = _config_parser.get(label, key).format(label, key).replace('model',
+                                                                              f'{bp_model}{rp_model}')
     file_name = file_name.replace('system', system) if system else file_name.replace('system_', '')
     return file_name
 
 
 def get_file(label, key, system, bp_model, rp_model, config_file=None):
     """
     Get the file path corresponding to the given label and key.
@@ -73,14 +73,15 @@
     """
     Load the XpMerge table from the filter XML file.
 
     Args:
         system (str): Name of the photometric system if it corresponds.
         bp_model (str): BP model.
         rp_model (str): RP model.
+        config_file (str): Path to configuration file.
 
     Returns:
         ndarray: Array containing the sampling grid values.
         dict: A dictionary containing the XpMerge table with one entry for BP and one for RP.
     """
     bp_model = bp_model if bp_model else 'v375wi'
     label = key = 'filter'
@@ -94,14 +95,15 @@
     """
     Load the XpSampling table from the XML filter file.
 
     Args:
         system (str): Photometric system name, can be None in which case the generic configuration is loaded.
         bp_model (str): BP model.
         rp_model (str): RP model.
+        config_file (str): Path to configuration file.
 
     Returns:
         dict: A dictionary containing the XpSampling table with one entry for BP and one for RP.
     """
     bp_model = bp_model if bp_model else 'v375wi'
     xml_file = get_file('filter', 'filter', system, bp_model, rp_model, config_file=config_file)
     x_root = get_file_root(xml_file)
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/core/dispersion_function.py` & `gaiaxpy-2.1.1/src/gaiaxpy/core/dispersion_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import numpy as np
 import pandas as pd
 from scipy import interpolate
 
 from gaiaxpy.config.paths import config_path, config_ini_file
 from gaiaxpy.core.satellite import BANDS, BP_WL, RP_WL
 
+
 @lru_cache(maxsize=None)
 def read_config_file():
     config_parser = ConfigParser()
     config_parser.read(config_ini_file)
     config_file = join(config_path, config_parser.get('core', 'dispersion_function'))
     return pd.read_csv(config_file)
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/error_correction/error_correction.py` & `gaiaxpy-2.1.1/src/gaiaxpy/error_correction/error_correction.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 error_correction.py
 ====================================
 Module that implements the error correction over a multi-photometry.
 """
 
 from functools import lru_cache
 from os import listdir
-from os.path import join
+from os.path import join, isfile
+from sys import stdout
 
 import numpy as np
 import pandas as pd
 from scipy.interpolate import interp1d
 from tqdm import tqdm
 
 from gaiaxpy.config.paths import correction_tables_path
 from gaiaxpy.core.generic_functions import cast_output, _extract_systems_from_data, _warning
-from gaiaxpy.core.generic_variables import pbar_colour, pbar_units
+from gaiaxpy.core.generic_variables import pbar_colour, pbar_units, pbar_message
 from gaiaxpy.input_reader.input_reader import InputReader
 from gaiaxpy.output.photometry_data import PhotometryData
 
 
 @lru_cache(maxsize=None)
 def _get_correctable_systems():
     correction_files = listdir(correction_tables_path)
     systems = [filename.split('-')[2] for filename in correction_files]
     return systems
 
 
 def _read_system_table(system):
-    try:
-        correction_factors_path = join(correction_tables_path, f'DIDREQ-465-{system}-correction-factors.csv')
-        correction_table = pd.read_csv(correction_factors_path, float_precision='high')
-    except FileNotFoundError:
-        raise FileNotFoundError(f'No correction table found for system {system}.')
-    correction_table['bin_centre'] = (correction_table['min_Gmag_bin'] + correction_table['max_Gmag_bin']) / 2
-    return correction_table
+    correction_factors_path = join(correction_tables_path, f'DIDREQ-465-{system}-correction-factors.csv')
+    if isfile(correction_factors_path):
+        correction_table = pd.read_csv(correction_factors_path, float_precision='round_trip')
+        correction_table['bin_centre'] = (correction_table['min_Gmag_bin'] + correction_table['max_Gmag_bin']) / 2
+        return correction_table
+    raise FileNotFoundError(f'No correction table found for system {system}.')
 
 
 def _get_correction_array(_mag_G_values, system):
     correction_table = _read_system_table(system)
     min_value, max_value = correction_table['min_Gmag_bin'].iloc[0], correction_table['max_Gmag_bin'].iloc[-1]
     floor_mag_dict = correction_table.set_index('min_Gmag_bin').T.to_dict()
     factor_columns = [col for col in correction_table.columns if 'factor_' in col]
@@ -110,17 +110,18 @@
                                    output_path=output_path, output_file=output_file, output_format=output_format,
                                    save_file=save_file)
 
 
 def _apply_error_correction(input_multi_photometry, photometric_system=None, output_path='.',
                             output_file='output_corrected_photometry', output_format=None, save_file=True,
                             disable_info=False):
+    __FUNCTION_KEY = 'correction'
     gaia_system = 'GaiaDr3Vega'
     gaia_G_mag_column = f'{gaia_system}_mag_G'
-    input_multi_photometry, extension = InputReader(input_multi_photometry, apply_error_correction,
+    input_multi_photometry, extension = InputReader(input_multi_photometry, apply_error_correction, False,
                                                     disable_info=disable_info).read()
     # Validate that it is a multi-photometry, but how? First try below:
     if gaia_G_mag_column not in input_multi_photometry.columns:
         raise ValueError('System Gaia_DR3_Vega, required to apply the error correction is not present in the input'
                          ' photometry.')
     columns = list(input_multi_photometry.columns)
     columns.remove('source_id')
@@ -129,16 +130,16 @@
     systems = list(set(systems_in_data) & set(__correctable_systems))
     systems_to_skip = set(systems_in_data) - set(__correctable_systems)
     if systems_to_skip and not disable_info:
         print()
     for system in systems_to_skip:
         _warning(f'System {system} does not have a correction table. The program will not apply error correction over'
                  ' this system.')
-    for system in tqdm(systems, desc='Correcting systems', total=len(systems), unit=pbar_units['correction'],
-                       leave=False, colour=pbar_colour):
+    for system in tqdm(systems, desc=pbar_message[__FUNCTION_KEY], total=len(systems), unit=pbar_units[__FUNCTION_KEY],
+                       leave=False, colour=pbar_colour, file=stdout):
         system_df = input_multi_photometry[[column for column in input_multi_photometry.columns if
                                             (column.startswith(system) and f'{system}Std' not in column) or
                                             column == gaia_G_mag_column]]
         # Get the correction factors for the mag G column
         correction_array = _get_correction_array(system_df[gaia_G_mag_column], system)
         # Correct error magnitudes
         corrected_system = _correct_system(system_df, correction_array)
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/file_parser/cast.py` & `gaiaxpy-2.1.1/src/gaiaxpy/file_parser/cast.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 Module to cast the data after parsing.
 """
 import numpy as np
 from numpy.ma import MaskError, getdata
 from pandas.errors import IntCastingNaNError
 
 # Fields of all formats including AVRO.
-__type_map = {'source_id': 'int64', 'solution_id': 'int64', 'rp_n_parameters': 'int64', 'bp_n_parameters': 'int64',
-              'rp_n_rejected_measurements': 'int64', 'bp_n_rejected_measurements': 'int64',
-              'rp_n_measurements': 'int64', 'bp_n_measurements': 'int64',
-              'rp_standard_deviation': 'float64', 'bp_standard_deviation': 'float64',
-              'rp_num_of_transits': 'int64', 'bp_num_of_transits': 'int64',
-              'rp_num_of_blended_transits': 'int64', 'bp_num_of_blended_transits': 'int64',
-              'rp_num_of_contaminated_transits': 'int64', 'bp_num_of_contaminated_transits': 'int64',
+__type_map = {'source_id': 'Int64', 'solution_id': 'Int64',
+              'rp_n_parameters': 'Int16', 'bp_n_parameters': 'Int16',
+              'rp_n_rejected_measurements': 'Int64', 'bp_n_rejected_measurements': 'Int64',
+              'rp_n_measurements': 'Int64', 'bp_n_measurements': 'Int64',
+              'rp_standard_deviation': 'Float64', 'bp_standard_deviation': 'Float64',
+              'rp_num_of_transits': 'Int64', 'bp_num_of_transits': 'Int64',
+              'rp_num_of_blended_transits': 'Int64', 'bp_num_of_blended_transits': 'Int64',
+              'rp_num_of_contaminated_transits': 'Int64', 'bp_num_of_contaminated_transits': 'Int64',
               'rp_coefficients': 'O', 'bp_coefficients': 'O',
               'rp_coefficient_covariances': 'O', 'bp_coefficient_covariances': 'O',
-              'rp_degrees_of_freedom': 'int64', 'bp_degrees_of_freedom': 'int64',
-              'rp_n_relevant_bases': 'int64', 'bp_n_relevant_bases': 'int64',
-              'rp_basis_function_id': 'int64', 'bp_basis_function_id': 'int64',
-              'rp_chi_squared': 'float64', 'bp_chi_squared': 'float64',
+              'rp_degrees_of_freedom': 'Int64', 'bp_degrees_of_freedom': 'Int64',
+              'rp_n_relevant_bases': 'Int64', 'bp_n_relevant_bases': 'Int64',
+              'rp_basis_function_id': 'Int64', 'bp_basis_function_id': 'Int64',
+              'rp_chi_squared': 'Float64', 'bp_chi_squared': 'Float64',
               'rp_coefficient_errors': 'O', 'bp_coefficient_errors': 'O',
               'rp_coefficient_correlations': 'O', 'bp_coefficient_correlations': 'O',
-              'rp_relative_shrinking': 'float64', 'bp_relative_shrinking': 'float64'}
+              'rp_relative_shrinking': 'Float64', 'bp_relative_shrinking': 'Float64'}
 
 
 def __replace_masked_array(value):
     if (isinstance(value, np.ma.core.MaskedArray) and getdata(value).size == 0) or (isinstance(value, float) and
                                                                                     value == 0.0):
         return np.array([])
     elif isinstance(value, np.ma.core.MaskedArray):
@@ -45,24 +46,23 @@
 def _cast(df):
     """
     Cast types to the defined ones to standardise the different input formats.
 
     Args:
         df (DataFrame): a DataFrame with parsed data from input files.
     """
+    # flake8: noqa
     for column in ['bp_n_parameters', 'bp_basis_function_id']:
         if column in df.columns:
             df[column] = df[column].apply(lambda row: __replace_masked_constant(row))
     for column, type_value in __type_map.items():
         try:
             if type_value == 'O':
                 df[column] = df[column].apply(lambda x: __replace_masked_array(x))
-            # Only try to cast if required. If the type is float, it will just parse it. If it's already an int type,
-            # it will skip the casting
-            elif 'int' not in str(df[column].dtype).__str__().lower():
+            else:
                 df[column] = df[column].astype(type_value)
         except (TypeError, IntCastingNaNError):
             df[column] = df[column].astype(type_value.title())
         except KeyError:
             continue  # Not every key is available in every case
         except ValueError as err:
             if np.isnan(np.sum(df[column].values)):
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/file_parser/parse_generic.py` & `gaiaxpy-2.1.1/src/gaiaxpy/file_parser/parse_generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
 
 class GenericParser(object):
     """
     Generic spectra parser.
     """
 
+    def __init__(self):
+        self.info_msg = 'Reading input file...'
+
     def get_parser(self, extension):
         """
         Choose the parser to use based on the extension.
 
         Args:
             extension (str): File extension including the dot (e.g.: '.csv').
 
@@ -54,29 +57,33 @@
         elif extension == 'fits':
             return self._parse_fits
         elif extension == 'xml':
             return self._parse_xml
         else:
             raise InvalidExtensionError()
 
-    def _parse(self, file_path):
+    def parse_file(self, file_path, disable_info=False):
         """
         Parse the input file according to its extension.
 
         Args:
             file_path (str): Path to a file.
+            disable_info (bool): Whether to disable the progress tracker or not.
 
         Returns:
             DataFrame: Pandas DataFrame representing the file.
             str: File extension ('.csv', '.fits', or '.xml').
         """
-        print('Reading input file...', end='\r')
+        if not disable_info:
+            print(self.info_msg, end='\r')
         extension = _get_file_extension(file_path)
         parser = self.get_parser(extension)
         parsed_data = _cast(parser(file_path))
+        if not disable_info:
+            print(self.info_msg + ' Done!', end='\r')
         return parsed_data, extension
 
     def _parse_avro(self, avro_file):
         raise NotImplementedError('Method not implemented for base class.')
 
     def _parse_csv(self, csv_file, _array_columns=None, _matrix_columns=None, _usecols=None):
         """
@@ -88,15 +95,15 @@
             _matrix_columns (list of tuples): List of tuples where the first element is the number of rows/columns of a
                 square matrix which values are those contained in the second element of the tuple.
             _usecols (list): Columns to read.
 
         Returns:
             DataFrame: A pandas DataFrame representing the CSV file.
         """
-        df = pd.read_csv(csv_file, comment='#', float_precision='high', usecols=_usecols)
+        df = pd.read_csv(csv_file, comment='#', float_precision='round_trip', usecols=_usecols)
         if _array_columns:  # Pandas converters seemed slower
             for column in _array_columns:
                 if column in df.columns:
                     df[column] = df[column].apply(lambda x: str_to_array(x))
         if _matrix_columns:
             for size_column, values_column in _matrix_columns:
                 df[values_column] = df.apply(lambda row: array_to_symmetric_matrix(str_to_array(row[values_column]),
@@ -135,18 +142,18 @@
             _matrix_columns (list of tuples): List of tuples where the first element is the number of rows/columns of a
                 square matrix which values are those contained in the second element of the tuple.
             _usecols (list): Columns to read.
 
         Returns:
             DataFrame: A pandas DataFrame representing the XML file.
         """
-        # Astropy won't automatically remove the columns that are not in _usecols but it speeds up the process a bit
+        # Astropy won't automatically remove the columns that are not in _usecols, but it speeds up the process a bit
         table = Table.read(xml_file, columns=_usecols)
-        # Parsing only the required columns would be ideal, but not necessarily issue due to some type issues
-        df = table.to_pandas()[_usecols]
+        # The table read by Astropy will still contain all the columns
+        df = table.to_pandas()[_usecols] if _usecols else table.to_pandas()
         if _matrix_columns:
             for size_column, values_column in _matrix_columns:
                 df[values_column] = df.apply(lambda row: array_to_symmetric_matrix(row[values_column],
                                                                                    row[size_column]), axis=1)
         return df
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/file_parser/parse_inverse.py` & `gaiaxpy-2.1.1/src/gaiaxpy/file_parser/parse_inverse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 from typing import Union
 
-from gaiaxpy.core.generic_functions import _warning
 from gaiaxpy.file_parser.parse_generic import GenericParser
 
 
 class InverseBasesParser(GenericParser):
     """
     Parser for the inverse bases used in the external calibration.
     """
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/file_parser/utils.py` & `gaiaxpy-2.1.1/src/gaiaxpy/file_parser/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from functools import reduce
 
 
 def _get_from_dict(dictionary, _map):
     try:
         return reduce(operator.getitem, _map, dictionary)
     except TypeError:
-        return None
+        return float('NaN')
     except KeyError:
         raise KeyError(f'Element {_map} not found in AVRO dictionary. Is it an actual field in the input file?')
 
 
 # This dictionary contains the mapping from the usual CSV fields to the AVRO fields.
 _csv_to_avro_map = {'source_id': ['sourceId'],
                     'rp_n_rejected_measurements': ['rpSpec', 'solution', 'numberOfRejectedMeasurements'],
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/generator/config.py` & `gaiaxpy-2.1.1/src/gaiaxpy/generator/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from os import walk, urandom
 from os.path import isdir, join
 from re import match
 
 from gaiaxpy.core.config import ADDITIONAL_SYSTEM_PREFIX
 
 _CFG_FILE_PATH = join(tempfile.gettempdir(), urandom(24).hex())
+_ADDITIONAL_SYSTEM_FILES_REGEX = r'[a-zA-Z0-9-_]+\.gaiaxpy_dr3_[a-zA-Z0-9-]+\.xml'
 
 
 class GenCfg:
 
     def __init__(self, filters_dir: str, version: str):
         if not isdir(filters_dir):
             raise ValueError(f'{filters_dir} is not a path to a valid directory.')
@@ -29,14 +30,16 @@
 
     Returns:
         list: List of compliant file names.
 
     Raises:
         ValueError: If no compliant files are found in the given directory.
     """
+    if not isdir(dir_path):
+        raise ValueError('Input path is not a valid directory.')
     all_files = [f for _, _, fn in walk(dir_path) for f in fn]
     compliant_files = [f for f in all_files if __file_name_is_compliant(f)]
     if len(compliant_files) == 0:
         raise ValueError('No filter files found in the given directory. Please check your files.')
     elif len(compliant_files) < len(all_files) and show_warning:
         message = 'Some files in the directory do not correspond to filter files. The program will ignore them.'
         print(f'UserWarning: {message}', file=sys.stderr)
@@ -49,16 +52,15 @@
 
     Args:
         file_name (str): Name of the file.
 
     Returns:
         bool: True if the file name is compliant, False otherwise.
     """
-    regex = '[a-zA-Z0-9-_]+\.gaiaXPy_dr3_[a-zA-Z0-9-]+\.xml'
-    return match(regex, file_name) is not None
+    return match(_ADDITIONAL_SYSTEM_FILES_REGEX, file_name.lower()) is not None
 
 
 def create_config(systems_path: str = None, config_file: str = None):
     """
     Creates a configuration file with the provided `systems_path` and `config_file` parameters.
     If `systems_path` is not provided, it will prompt the user to enter it.
     The configuration file contains the path to the additional systems directory and the version of the additional
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/generator/internal_photometric_system.py` & `gaiaxpy-2.1.1/src/gaiaxpy/generator/internal_photometric_system.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 internal_photometric_system.py
 ====================================
 Module for the parent class of the standardised and regular photometric systems.
 """
+import re
 from configparser import ConfigParser
 from glob import glob
 from os import remove
-from os.path import exists
+from os.path import exists, split, join
 
+from gaiaxpy.core.version import __version__
 from gaiaxpy.config.paths import config_ini_file
-from gaiaxpy.core.config import get_filter_version_from_config, replace_file_name, get_file_path, \
-    ADDITIONAL_SYSTEM_PREFIX
+from gaiaxpy.core.config import (get_filter_version_from_config, replace_file_name, get_file_path,
+                                 ADDITIONAL_SYSTEM_PREFIX)
 from gaiaxpy.core.generic_functions import _get_system_label
 from gaiaxpy.core.satellite import BANDS
-from gaiaxpy.core.version import __version__
 from gaiaxpy.core.xml_utils import get_file_root, parse_array, get_array_text, get_xp_sampling_matrix, get_xp_merge
-from .config import _CFG_FILE_PATH
+from .config import _CFG_FILE_PATH, _ADDITIONAL_SYSTEM_FILES_REGEX
 
 
 class InternalPhotometricSystem(object):
 
     def __init__(self, name: str, config_file: str = None, bp_model: str = 'v375wi', rp_model: str = 'v142r'):
         self.label = _get_system_label(name)
         self.version = None
@@ -109,18 +110,28 @@
         Args:
             bp_model (str): BP model.
             rp_model (str): RP model.
 
         Returns:
             str: Path of a file.
         """
+
+        def _validate_additional_system_file(_actual_path):
+            file_names = [split(p)[1] for p in _actual_path]
+            pattern = re.compile(_ADDITIONAL_SYSTEM_FILES_REGEX, re.IGNORECASE)
+            if all(f.startswith('XpFilter') for f in file_names):
+                return _actual_path
+            return [join(file_path, s) for s in file_names if pattern.match(s) and not s.startswith('XpFilter')]
+
         file_name = replace_file_name(self.config_file, 'filter', 'filter', bp_model, rp_model, self.label)
+        system_name = file_name.split('.')[0]
         file_path = get_file_path(self.config_file)
         # Search file in file path to obtain the actual path
-        actual_path = glob(file_path + f"/**/{file_name}", recursive=True)
+        actual_path = glob(file_path + f"/**/{system_name}*.xml", recursive=True)
+        actual_path = _validate_additional_system_file(actual_path)
         if len(actual_path) == 0:
             raise ValueError('Filter file not found in given path.')
         elif len(actual_path) > 1:
             # Remove configuration file if it exists to avoid issues on reloading
             if exists(_CFG_FILE_PATH):
                 remove(_CFG_FILE_PATH)
             raise ValueError(f'More than one system named {self.label.replace(f"{ADDITIONAL_SYSTEM_PREFIX}_", "")}'
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/generator/photometric_system.py` & `gaiaxpy-2.1.1/src/gaiaxpy/generator/photometric_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,18 @@
     print('Systems loaded. Use PhotometricSystem.get_available_systems() to get the names of the current available'
           ' systems.')
     return updated_enum
 
 
 def __load_additional_systems(_filters_path=None, config_file=None):
     """
-    Load additional photometric systems. These name of these additional systems will start with the prefix USER.
+    Load additional photometric systems. The names of these additional systems will start with the prefix 'USER.'
+    For example, if a system is named 'X' in the loaded file, the corresponding photometric system will be referenced
+    in GaiaXPy as 'USER_X', and it should be called using 'PhotometricSystem.USER_X,' where USER is not a username but
+    simply the string 'USER'.
 
     Args:
         _filters_path (str): Path to directory containing the additional filter files.
         config_file (str): Path to configuration file where the path to the additional filter files will be stored.
     """
     config_file = config_file if config_file else _CFG_FILE_PATH
     if exists(config_file) and contains_filter_key(config_file):
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/generator/regular_photometric_system.py` & `gaiaxpy-2.1.1/src/gaiaxpy/generator/regular_photometric_system.py`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/generator/standardised_photometric_system.py` & `gaiaxpy-2.1.1/src/gaiaxpy/generator/standardised_photometric_system.py`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/generator/synthetic_photometry_generator.py` & `gaiaxpy-2.1.1/src/gaiaxpy/generator/synthetic_photometry_generator.py`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/generator/utils.py` & `gaiaxpy-2.1.1/src/gaiaxpy/generator/utils.py`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/input_reader/dataframe_string_array_reader.py` & `gaiaxpy-2.1.1/src/gaiaxpy/input_reader/dataframe_string_array_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def _parse_brackets_arrays(self):
         df = self.content
         array_columns = self.array_columns
         for column in array_columns:
             df[column] = df[column].map(np.array)
         return df
 
-    def _parse(self):
+    def read(self):
         def __get_enclosing_element(_df, _array_columns):
             for row in _df.to_dict('records'):
                 for column in _array_columns:
                     if isinstance(row[column], str):
                         if row[column][0] in ['(', '[']:
                             return row[column][0]
                     else:
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/input_reader/list_reader.py` & `gaiaxpy-2.1.1/src/gaiaxpy/input_reader/list_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 from astroquery.gaia import GaiaClass
 
 from gaiaxpy.core.server import data_release, gaia_server
 from .archive_reader import ArchiveReader
 from .dataframe_reader import DataFrameReader
+from ..core.custom_errors import SelectorNotImplementedError
 
-not_supported_functions = ['apply_colour_equation', 'apply_error_correction', 'simulate_continuous', 'simulate_sampled']
+not_supported_functions = ['apply_colour_equation', 'apply_error_correction']
 
 
 def extremes_are_enclosing(first_row, column):
     if first_row[column][0] == '[' and first_row[column][-1] == ']':
         return True
     elif first_row[column][0] == '(' and first_row[column][-1] == ')':
         return True
     else:
         return False
 
 
 class ListReader(ArchiveReader):
 
-    def __init__(self, content, function, user, password, disable_info=False):
-        super(ListReader, self).__init__(function, user, password)
+    def __init__(self, content, function, truncation, user, password, additional_columns=None, selector=None,
+                 disable_info=False):
+        if selector is not None:
+            raise SelectorNotImplementedError('List')
+        if additional_columns is None:
+            additional_columns = dict()
+        super(ListReader, self).__init__(function, truncation, user, password, additional_columns=additional_columns,
+                                         disable_info=disable_info)
         if content:
             self.content = content
         else:
             raise ValueError('Input list cannot be empty.')
         self.disable_info = disable_info
 
     def read(self, _data_release=data_release):
-        # TODO: list could contain elements that are not sourceIds
         sources = self.content
         function_name = self.function.__name__
         if function_name in not_supported_functions:
             raise ValueError(f'Function {function_name} does not support receiving a list as input.')
         # Connect to geapre
         gaia = GaiaClass(gaia_tap_server=gaia_server, gaia_data_server=gaia_server)
         self._login(gaia)
         # ADQL query
         if not self.disable_info:
-            print('Running query...', end='\r')
+            print(self.info_msg, end='\r')
         result = gaia.load_data(ids=sources, format='csv', data_release=_data_release, data_structure='raw',
                                 retrieval_type='XP_CONTINUOUS', avoid_datatype_check=True)
         try:
             continuous_key = [key for key in result.keys() if 'continuous' in key.lower()][0]
             data = result[continuous_key][0].to_pandas()
         except (KeyError, IndexError):
             raise ValueError('No continuous raw data found for the given sources.')
-        return DataFrameReader(data).read_df()
+        if not self.disable_info:
+            print(self.info_msg + ' Done!', end='\r')
+        return DataFrameReader(data, function_name, self.truncation, additional_columns=self.additional_columns,
+                               disable_info=True).read()
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/output/continuous_spectra_data.py` & `gaiaxpy-2.1.1/src/gaiaxpy/output/continuous_spectra_data.py`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/output/output_data.py` & `gaiaxpy-2.1.1/src/gaiaxpy/output/output_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,73 +6,42 @@
 from ast import literal_eval
 from os.path import dirname, abspath, join
 
 from gaiaxpy.core.generic_functions import standardise_extension
 from gaiaxpy.file_parser.parse_generic import InvalidExtensionError
 
 
+def _initialise_header():
+    return ["# %ECSV 1.0", "# ---", "# delimiter: ','", "# datatype:"]
+
+
 def _load_header_dict():
     current_path = dirname(abspath(__file__))
     header_dictionary_path = join(current_path, 'ecsv_headers', 'headers_dict.txt')
     with open(header_dictionary_path) as f:
         data = f.read()
     # Load header dictionary
     header_dict = literal_eval(data)
     return header_dict
 
 
 def _build_regular_header(columns):
     header_dict = _load_header_dict()
     header = _initialise_header()
     for column in columns:
+        current_column = header_dict[column]
         header.append('# -')
         header.append(f'#   name: {column}')
-        header.append(f'#   datatype: {header_dict[column]["datatype"]}')
-        try:
-            header.append(f'#   subtype: {header_dict[column]["subtype"]}')
-        except KeyError:
-            pass
-        header.append(f'#   description: {header_dict[column]["description"]}')
-    return '\n'.join(header) + '\n'
-
-
-def _initialise_header():
-    return ["# %ECSV 1.0", "# ---", "# delimiter: ','", "# datatype:"]
-
-
-def _build_photometry_header(columns):
-    header_dict = _load_header_dict()
-    header = _initialise_header()
-    for column in columns:
-        header.append('# -')
-        header.append(f'#   name: {column}')
-        if column != 'source_id':
-            if '_flux_error_' in column:
-                parameter = '_flux_error_'
-            elif '_flux_' in column:
-                parameter = '_flux_'
-            elif '_mag_' in column:
-                parameter = '_mag_'
-            system, band = column.split(parameter)
-            parameter = f'phot{parameter}'[:-1]
-            header.append(f'#   datatype: {header_dict[parameter]["datatype"]}')
-            header.append(f'#   description: {header_dict[parameter]["description"]} {band} band')
-        else:
-            header.append(f'#   datatype: {header_dict[column]["datatype"]}')
-            header.append(f'#   description: {header_dict[column]["description"]}')
+        header.append(f'#   datatype: {current_column["datatype"]}')
+        if current_column.get('subtype'):
+            header.append(f'#   subtype: {current_column["subtype"]}')
+        header.append(f'#   description: {current_column["description"]}')
     return '\n'.join(header) + '\n'
 
 
-def _add_header(header, output_path, output_file):
-    with open(join(output_path, f'{output_file}.ecsv'), "r+") as f:
-        s = f.read()
-        f.seek(0)
-        f.write(header + s)
-
-
 class OutputData(object):
 
     def __init__(self, data, positions):
         self.data = data.copy()
         self.positions = positions
 
     def save(self, save_file, output_path, output_file, output_format, extension):
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/output/photometry_data.py` & `gaiaxpy-2.1.1/src/gaiaxpy/output/photometry_data.py`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/output/sampled_spectra_data.py` & `gaiaxpy-2.1.1/src/gaiaxpy/output/sampled_spectra_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 Module to represent a dataframe of sampled spectra.
 """
 
 import warnings
 from os.path import join
 from pathlib import Path
 
-import numpy as np
 import pandas as pd
 from astropy.io import fits
-from astropy.io.votable.tree import Field, Param, Resource, Table, VOTableFile
+from astropy.io.votable.tree import Field, Param, Resource, VOTableFile
 from astropy.units import UnitsWarning
 from fastavro import parse_schema, writer
 from fastavro.validation import validate_many
 from numpy import ndarray
 
 from .output_data import OutputData
-from .utils import _add_ecsv_header, _array_to_standard, _build_ecsv_header, _generate_fits_header, \
-    _get_sampling_dict, _load_header_dict
+from .utils import (_add_ecsv_header, _array_to_standard, _build_ecsv_header, _generate_fits_header,
+                    _get_sampling_dict, _load_header_dict, _get_col_subtype_len)
 
-warnings.filterwarnings('ignore', category=UnitsWarning)
+try:
+    from astropy.io.votable.tree import TableElement as ATable
+except ImportError:
+    from astropy.io.votable.tree import Table as ATable
 
 
 class SampledSpectraData(OutputData):
 
     def __init__(self, data, positions):
         super().__init__(data, positions)
 
@@ -77,19 +79,16 @@
                 return [{'name': key, 'type': field_to_type[key]} for key in keys]
 
             schema = {'doc': 'Spectrum output.', 'name': 'Spectra', 'namespace': 'spectrum', 'type': 'record',
                       'fields': build_field(_spectra_dicts[0].keys()), }
             # Spectrum fields to string
             for spectrum in _spectra_dicts:
                 for field, _type in field_to_type.items():
-                    if _type == 'string' and not field == 'xp':
-                        try:
-                            spectrum[field] = str(tuple(spectrum[field]))
-                        except KeyError:
-                            continue  # Key may not exist (e.g.: 'xp')
+                    if _type == 'string' and field in spectrum.keys() and not field == 'xp':
+                        spectrum[field] = str(tuple(spectrum[field]))
             # Validate that records match the schema
             validate_many(_spectra_dicts, schema)
             return parse_schema(schema), _spectra_dicts
 
         data = self.data
         positions = self.positions
         Path(output_path).mkdir(parents=True, exist_ok=True)
@@ -139,42 +138,50 @@
         """
         Save the output data in FITS format.
 
         Args:
             output_path (str): Path where to save the file.
             output_file (str): Name of the output file.
         """
+        warnings.filterwarnings('ignore', category=UnitsWarning)
+
+        def _flux_contains_none(arrays):
+            return any(arr is None for arr in arrays['flux'])
+
         data = self.data
         positions = self.positions
-        # Get length of flux (should be the same as length of error)
-        flux_format = f'{len(positions)}D'  # D: double precision float
-        flux_error_format = f'{len(positions)}E'  # E: single precision float
-        correlation_format = ''  # Correlation if requested
-        try:
-            correlation_format = f"{len(data['correlation'].iloc[0])}D"
-        except KeyError:
-            pass
-        # Define formats for each type according to FITS
-        column_formats = {'source_id': 'K', 'xp': '2A', 'flux': flux_format, 'flux_error': flux_error_format,
-                          'correlation': correlation_format, 'standard_deviation': 'E'}
-        # create a list of HDUs
+        # Create a list of HDUs
         hdu_list = list()
         # create a header to include the sampling
         hdr = fits.Header()
         primary_hdu = fits.PrimaryHDU(header=hdr)
         hdu_list.append(primary_hdu)
         # Create a dictionary to hold all the data
         output_by_column_dict = data.reset_index().to_dict(orient='list')
         # Remove index from output dict
         output_by_column_dict.pop('index', None)
         spectra_keys = output_by_column_dict.keys()
         data_type = data.attrs['data_type']
         units_dict = data_type.get_units()
-        columns = [fits.Column(name=key, array=np.array(output_by_column_dict[key]), format=column_formats[key],
-                               unit=units_dict.get(key, '')) for key in spectra_keys]
+        pos_len = len(positions)
+        contains_none = _flux_contains_none(output_by_column_dict)
+        # D: double precision float
+        flux_format = 'PD()' if contains_none else f'{pos_len}D'
+        # E: single precision float
+        flux_error_format = 'PE()' if contains_none else f'{pos_len}E'
+        aux_corr = data.get('correlation')
+        correlation_format = ''
+        if aux_corr is not None:
+            correlation_format = 'PD()' if contains_none else f"{_get_col_subtype_len(data, 'correlation')}D"
+        # Define formats for each type according to FITS
+        column_formats = {'source_id': 'K', 'xp': '2A', 'flux': flux_format, 'flux_error': flux_error_format,
+                          'correlation': correlation_format, 'standard_deviation': 'E'}
+        columns = [
+            fits.Column(name=key, array=[value if value is not None else [] for value in output_by_column_dict[key]],
+                        format=column_formats[key], unit=units_dict.get(key, '')) for key in spectra_keys]
         header = _generate_fits_header(data, column_formats)
         header['Sampling'] = str(tuple(positions))
         hdu = fits.BinTableHDU.from_columns(columns, header=header)
         hdu_list.append(hdu)
         # Put all HDUs together
         hdul = fits.HDUList(hdu_list)
         # Write the file and replace it if it already exists
@@ -186,26 +193,29 @@
         """
         Save the output spectra in XML/VOTABLE format.
 
         Args:
             output_path (str): Path where to save the file.
             output_file (str): Name of the output file.
         """
+        warnings.filterwarnings('ignore', category=UnitsWarning)
 
         def _create_params(_votable, sampling, data_type):
             column = 'sampling'
             unit = data_type.get_units().get('pos', '')
             return [Param(_votable, name=column, ID=f'_{column}', ucd='em.wl', datatype='double', arraysize='*',
                           unit=unit, value=list(sampling))]
 
         def _create_fields(_votable, _spectra_df):
-            len_flux = str(len(_spectra_df['flux'].iloc[0]))
-            len_error = str(len(_spectra_df['flux_error'].iloc[0]))
-            len_correlation = str(len(_spectra_df['correlation'].iloc[0])) \
-                if 'correlation' in _spectra_df.columns else ''
+            _spectra_flux_len = _get_col_subtype_len(_spectra_df, 'flux')
+            _spectra_flux_error_len = _get_col_subtype_len(_spectra_df, 'flux_error')
+            len_flux = str(_spectra_flux_len)
+            len_error = str(_spectra_flux_error_len)
+            len_correlation = str(
+                len(_spectra_df['correlation'].iloc[0])) if 'correlation' in _spectra_df.columns else ''
             fields_datatypes = {'source_id': 'long', 'xp': 'char', 'flux': 'double', 'flux_error': 'float',
                                 'correlation': 'double', 'standard_deviation': 'float'}
             fields_array_size = {'source_id': '', 'xp': '2', 'flux': len_flux, 'flux_error': len_error,
                                  'correlation': len_correlation, 'standard_deviation': ''}
             fields_id = {key: f'_{key}' for key in ['source_id', 'xp', 'flux', 'flux_error', 'correlation']}
             fields_id.update({'source_id': None})
             header_dict = _load_header_dict()
@@ -227,15 +237,15 @@
         positions = list(self.positions)
         # Create a new VOTable file
         votable = VOTableFile()
         # Add a resource
         resource = Resource()
         votable.resources.append(resource)
         # Add a table for the spectra (and add the sampling as metadata)
-        spectra_table = Table(votable)
+        spectra_table = ATable(votable)
         resource.tables.append(spectra_table)
         # Add sampling as param
         params = _create_params(votable, positions, spectra_df.attrs['data_type'])
         spectra_table.params.extend(params)
         # Add spectrum fields
         fields = _create_fields(votable, spectra_df)
         spectra_table.fields.extend(fields)
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/output/utils.py` & `gaiaxpy-2.1.1/src/gaiaxpy/output/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     Args:
         array (ndarray): An array of floats.
         extension (str): Format to use 'csv' means use round brackets, 'ecsv' means use square brackets.
 
     Returns:
         tuple: The array converted to a tuple.
     """
+    if array is None:
+        return array
     if not isinstance(array, ndarray):
         raise ValueError('Input must be a NumPy array.')
 
     def convert_ecsv(row):
         # Square brackets should be used and nan values should be shown as null (no quotes)
         if np.isnan(np.min(row)):
             return '[' + ', '.join(['null' if np.isnan(value) else str(value) for value in row]) + ']'
@@ -55,36 +57,44 @@
     with open(header_dictionary_path) as f:
         data = f.read()
     # Load header dictionary
     header_dict = literal_eval(data)
     return header_dict
 
 
+def _get_col_subtype_len(_df, _column):
+    for index in range(0, len(_df)):
+        try:
+            return len(_df[_column].iloc[index])
+        except TypeError:
+            pass
+    raise ValueError('All arrays in the data seem to be empty. This should never happen.')
+
+
 def _build_ecsv_header(df, positions=None):
-    positions = str(list(positions)) if positions is not None else None
+    positions = None if positions is None else str(list(positions))
     columns = df.columns
     header_dict = _load_header_dict()
     header = _initialise_header()
     data_type = df.attrs['data_type']
     units_dict = data_type.get_units()
     for column in columns:
+        current_column = header_dict[column]
         header.append('# -')
         header.append(f'#   name: {column}')
-        header.append(f'#   datatype: {header_dict[column]["datatype"]}')
-        try:
+        header.append(f'#   datatype: {current_column["datatype"]}')
+        if 'subtype' in current_column.keys():
             header.append(
-                f'#   subtype: {header_dict[column]["subtype"].replace("null", str(len(df[column].iloc[0])))}')
-        except KeyError:
-            pass
-        header.append(f'#   description: {header_dict[column]["description"]}')
+                f'#   subtype: {current_column["subtype"].replace("null", str(_get_col_subtype_len(df, column)))}')
+        header.append(f'#   description: {current_column["description"]}')
         if units_dict.get(column, None):
             header.append(f'#   unit: {units_dict[column]}')
-        if header_dict[column].get('meta', None):
+        if current_column.get('meta', None):
             header.append('#   meta:')
-            header.append(f'#     ucd: {header_dict[column]["meta"]}')
+            header.append(f'#     ucd: {current_column["meta"]}')
     if positions:
         header.append('# meta:')
         header.append(f'#   sampling: {positions}')
     return '\n'.join(header) + '\n'
 
 
 def _initialise_header():
@@ -130,7 +140,18 @@
         cards.append((f'TTYPE{index + 1}', column))
         cards.append((f'TFORM{index + 1}', _column_formats.get(column, '')))
         cards.append((f'TCOMM{index + 1}', header_dict.get(column, dict()).get('description', '')))
         cards.append((f'TUCD{index + 1}', header_dict.get(column, dict()).get('meta', '')))
         cards.append((f'TUNIT{index + 1}', units_dict.get(column, '')))
     header = fits.Header(cards=cards)
     return header
+
+
+def _build_line_header(columns):
+    header_dict = _load_header_dict()
+    header = _initialise_header()
+    for column in columns:
+        header.append('# -')
+        header.append(f'#   name: {column}')
+        header.append(f'#   datatype: {header_dict[column]["datatype"]}')
+        header.append(f'#   description: {header_dict[column]["description"]}')
+    return '\n'.join(header) + '\n'
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/plotter/multi_absolute.py` & `gaiaxpy-2.1.1/src/gaiaxpy/plotter/multi_absolute.py`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/plotter/multi_xp.py` & `gaiaxpy-2.1.1/src/gaiaxpy/plotter/multi_xp.py`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/plotter/plot_spectra.py` & `gaiaxpy-2.1.1/src/gaiaxpy/plotter/plot_spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .multi_xp import MultiXpPlotter
 from .single import SinglePlotter
 
 
 def __plot_multi(spectra_type: str, spectra: pd.DataFrame, sampling: ndarray, show_plot: bool,
                  output_path: Optional[Union[Path, str]], output_file: Optional[str], format: str, legend: bool,
                  save_file: bool):
-    if spectra_type == 'AbsoluteSampledSpectrum':
+    if 'AbsoluteSampledSpectrum' in spectra_type:
         plotter = MultiAbsolutePlotter(spectra, sampling, show_plot, output_path, output_file, format,
                                        legend, save_file)
     elif spectra_type == 'XpSampledSpectrum':
         plotter = MultiXpPlotter(spectra, sampling, show_plot, output_path, output_file, format, legend, save_file)
     else:
         raise ValueError('Unrecognised spectra type.')
     return plotter
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/plotter/plotter.py` & `gaiaxpy-2.1.1/src/gaiaxpy/plotter/plotter.py`

 * *Files identical despite different names*

### Comparing `GaiaXPy-2.1.0/gaiaxpy/plotter/single.py` & `gaiaxpy-2.1.1/src/gaiaxpy/plotter/single.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
     def plot_fig(self):
         n_spectra = len(self.spectra)
         if n_spectra > self.max_spectra_on_single:
             raise ValueError(
                 f'Spectra list is too long. This functionality can only show up to {self.max_spectra_on_single} '
                 f'single plots. Try saving the plots without showing them using the option output_path.')
-        for index, spectrum in enumerate(self.spectra.to_dict('records')):
+        records = self.spectra.to_dict('records')
+        is_len_1 = len(records) == 1
+        for index, spectrum in enumerate(records):
             self._plot_single(spectrum)
             if self.save_file:
+                index = index if not is_len_1 else None
                 self._save_figure(index=index)
             if self.show_plot:
                 plt.show()
         plt.close()
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/spectrum/absolute_sampled_spectrum.py` & `gaiaxpy-2.1.1/src/gaiaxpy/spectrum/absolute_sampled_spectrum.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 Module to represent an absolute sampled spectrum.
 """
 
 from numbers import Number
 
 import numpy as np
 
-from gaiaxpy.core.satellite import BANDS, BP_WL, RP_WL
 from .sampled_spectrum import SampledSpectrum
 from .utils import _list_to_array
+from ..core.custom_errors import NoBandsAvailableError
 from ..core.generic_functions import correlation_from_covariance
 
 
 class AbsoluteSampledSpectrum(SampledSpectrum):
     """
     A spectrum calibrated onto the absolute system of wavelength and flux. The spectrum is represented by a set of
     discrete measurements or samples.
@@ -34,30 +34,33 @@
             truncation (dict): Number of bases to be used for this spectrum. The set of bases functions used for the
                 continuous representation of the spectra has been optimised to ensure that the first bases are the ones
                 that contribute most. In many cases, the last bases contribution will be below the noise. Truncation of
                 the basis function set to preserve only the significant bases is optional. By default, no truncation
                 will be applied, i.e. all bases will be used.
             with_correlation (bool): Whether correlation information should be computed.
         """
-        truncation = dict() if truncation is None else truncation
-        # Bands available
-        available_bands = [band for band in xp_spectra.keys() if xp_spectra[band].covariance is not None]
-        if not available_bands:
-            raise ValueError('At least one band must be present.')
-        pos = sampled_bases[available_bands[0]].get_sampling_grid()
+        self.truncation = dict() if truncation is None else truncation
+        self.available_bands = self.get_available_bands(xp_spectra)
+        if not self.available_bands:
+            raise NoBandsAvailableError()
+        pos = sampled_bases[self.available_bands[0]].get_sampling_grid()
         SampledSpectrum.__init__(self, source_id, pos)
-        self.pos = pos  # TODO: may not be required
-        split_spectrum = self.__generate_spectra(xp_spectra, sampled_bases, available_bands, truncation,
-                                                 with_correlation=with_correlation)
-        self.__merge_output(split_spectrum, merge, with_correlation=with_correlation)
-
-    def __generate_spectra(self, xp_spectra, sampled_bases, available_bands, truncation, with_correlation):
-        split_spectrum = {band: dict() for band in available_bands}
-        for band in available_bands:
-            band_truncation = truncation.get(band)
+        self.pos = pos
+
+    @staticmethod
+    def get_available_bands(xp_spectra):
+        def __is_available_band(_xp_spectra, band):
+            return isinstance(_xp_spectra[band].covariance, np.ndarray)
+
+        return [band for band in xp_spectra.keys() if __is_available_band(xp_spectra, band)]
+
+    def generate_spectra(self, xp_spectra, sampled_bases, with_correlation):
+        split_spectrum = {band: dict() for band in self.available_bands}
+        for band in self.available_bands:
+            band_truncation = self.truncation.get(band)
             split_spectrum[band]['xp_spectra'] = xp_spectra[band]
             stdev = split_spectrum[band]['xp_spectra'].get_standard_deviation()
             design_matrix = sampled_bases[band].get_design_matrix()
             spectra_covariance = split_spectrum[band]['xp_spectra'].get_covariance()
             coefficients = split_spectrum[band]['xp_spectra'].get_coefficients()
             if isinstance(band_truncation, Number) and band_truncation > 0:
                 design_matrix = design_matrix[:band_truncation][:]
@@ -67,46 +70,15 @@
             split_spectrum[band]['error'] = self._sample_error(spectra_covariance, design_matrix, stdev)
             if with_correlation:
                 split_spectrum[band]['cov'] = self._sample_covariance(spectra_covariance, design_matrix)
                 split_spectrum[band]['stdev'] = stdev
         return split_spectrum
 
     def __merge_output(self, split_spectrum, merge, with_correlation):
-        n_bands = len(split_spectrum.keys())
-        # If both bands are present
-        if n_bands == 2:
-            self.flux = np.add(np.multiply(split_spectrum[BANDS.bp]['flux'], merge[BANDS.bp]),
-                               np.multiply(split_spectrum[BANDS.rp]['flux'], merge[BANDS.rp]))
-            self.error = np.sqrt(np.add(np.multiply(split_spectrum[BANDS.bp]['error'] ** 2, merge[BANDS.bp] ** 2),
-                                        np.multiply(split_spectrum[BANDS.rp]['error'] ** 2, merge[BANDS.rp] ** 2)))
-            if with_correlation:
-                self.covariance = np.add(np.multiply(split_spectrum[BANDS.bp]['cov'], merge[BANDS.bp]),
-                                         np.multiply(split_spectrum[BANDS.rp]['cov'], merge[BANDS.rp]))
-        # If only one is
-        elif n_bands == 1:
-            existing_band, spectrum = list(split_spectrum.items())[0]
-            self.flux = spectrum['flux']
-            self.error = spectrum['error']
-            if with_correlation:
-                self.covariance = spectrum['cov']
-            # Patch values if there's a band missing
-            masked_pos = self.pos.copy()
-            masked_pos = masked_pos.astype(float)
-            if existing_band == BANDS.rp:
-                masked_pos[masked_pos <= RP_WL.low] = np.nan
-            elif existing_band == BANDS.bp:
-                masked_pos[masked_pos >= BP_WL.high] = np.nan
-            else:
-                raise ValueError(f'Band {existing_band} is not a valid band.')
-            # Get the indices of all the values in pos that are smaller than the lowest RP range value
-            self.flux[np.argwhere(np.isnan(masked_pos))] = np.nan
-            self.error[np.argwhere(np.isnan(masked_pos))] = np.nan
-            if with_correlation:
-                self.covariance[:, np.argwhere(np.isnan(masked_pos))] = np.nan
-                self.covariance[np.argwhere(np.isnan(masked_pos)), :] = np.nan
+        raise NotImplementedError('Method not implemented for base class.')
 
     def _get_fluxes(self):
         return self.flux
 
     def _get_flux_errors(self):
         return self.error
 
@@ -121,27 +93,27 @@
     def get_flux_label(cls):
         return 'Flux [W nm^-1 m^-2]'
 
     @classmethod
     def get_position_label(cls):
         return 'Wavelength [nm]'
 
-    def spectrum_to_dict(self):
+    def spectrum_to_dict(self, with_correlation):
         """
         Represent the spectrum as a dictionary.
 
         Returns:
             dict: A dictionary populated with the minimum set of parameters that need to be stored for this object.
                 This is optimised for writing large number of sampled spectra and for this reason the array of positions
                 is NOT included as it is expected to be the same for a batch of spectra. The array of positions can be
                 retrieved calling the sampling_to_dict method.
         """
         spectrum_dict = {'source_id': self.source_id, 'flux': _list_to_array(self.flux),
                          'flux_error': _list_to_array(self.error)}
-        if self.covariance is not None:
+        if with_correlation:
             full_correlation = correlation_from_covariance(self.covariance)
             spectrum_dict['correlation'] = full_correlation[np.tril_indices(full_correlation.shape[0], k=-1)]
         return spectrum_dict
 
     def _sampling_to_dict(self):
         """
         Represent the sampling grid as a dictionary.
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/spectrum/generic_spectrum.py` & `gaiaxpy-2.1.1/src/gaiaxpy/spectrum/xp_spectrum.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
-generic_spectrum.py
+xp_spectrum.py
 ====================================
-Module to represent a generic spectrum.
+Module to represent a BP/RP spectrum.
 """
 
+from .generic_spectrum import Spectrum
 
-class Spectrum(object):
+
+class XpSpectrum(Spectrum):
     """
-    Base spectrum. Contain only the source ID.
+    A spectrum observed with one of the Gaia low-resolution photometers (Blue or Red Photometer, BP or RP).
     """
 
-    def __init__(self, source_id):
+    def __init__(self, source_id, xp):
         """
-        Initialise a spectrum.
+        Initialise an XP spectrum.
 
         Args:
-            source_id (str): Source identifier. Can be a Gaia source ID (long) or any other source identifier.
+            source_id (int/str): Source identifier.
+            xp (str): Gaia photometer, can be either 'bp' or 'rp'.
         """
-        self.source_id = source_id
+        Spectrum.__init__(self, source_id)
+        self.xp = xp
 
-    def get_source_id(self):
+    def get_xp(self):
         """
-        Get the source ID of the spectrum.
+        Get band.
 
         Returns:
-            str: Source identifier.
+            str: Photometer identifier. Either 'bp' or 'rp'.
         """
-        return self.source_id
+        return self.xp
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/spectrum/multi_synthetic_photometry.py` & `gaiaxpy-2.1.1/src/gaiaxpy/spectrum/multi_synthetic_photometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,25 +35,25 @@
         self.photometric_system = photometric_system
         # One element per source_id, each sub element corresponds to one photometric_system
         self.photometries = photometries
         self.source_ids = _get_source_ids(photometries)
         self.mags, self.fluxes, self.errors = _generate_variables(photometries)
 
     def _generate_output_df(self):
-        photometries_df = self._photometries_to_dict()
+        photometries_df = self._photometries_to_df()
         # Reorder DataFrame columns
         phot_system_labels = [phot_system.get_system_label() for phot_system in self.photometric_system]
         reordered_columns = ['source_id']
         for label in phot_system_labels:
             column_sublist = [column for column in photometries_df.columns if column.startswith(f'{label}_')]
             reordered_columns.extend(column_sublist)
         photometries_df = photometries_df[reordered_columns]
         return photometries_df
 
-    def _photometries_to_dict(self):
+    def _photometries_to_df(self):
         list_of_dicts = []
         for source_id, mags, fluxes, errors in zip(self.source_ids, self.mags, self.fluxes, self.errors):
             phot = {'source_id': source_id}
             mag = self._field_to_dict(mags, 'mag')
             flux = self._field_to_dict(fluxes, 'flux')
             error = self._field_to_dict(errors, 'flux_error')
             list_of_dicts.append({**phot, **mag, **flux, **error})
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/spectrum/sampled_basis_functions.py` & `gaiaxpy-2.1.1/src/gaiaxpy/spectrum/sampled_basis_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Module to represent a set of basis functions evaluated on a grid.
 """
 
 import functools
 import math
 
 import numpy as np
+from scipy.interpolate import BSpline
 from scipy.special import eval_hermite, gamma
 
 from gaiaxpy.core import nature, satellite
 
 sqrt_4_pi = np.pi ** (-0.25)
 
 
@@ -46,44 +47,44 @@
             external_instrument_model (obj): external calibration instrument model. This object contains information on
                 the dispersion, response and inverse bases.
 
         Returns:
             SampledBasisFunctions: An instance of this class.
         """
         n_samples = len(sampling)
-        scale = (external_instrument_model.bases['normRangeMax'][0] -
-                 external_instrument_model.bases['normRangeMin'][0]) / \
-                (external_instrument_model.bases['pwlRangeMax'][0] -
-                 external_instrument_model.bases['pwlRangeMin'][0])
-        offset = external_instrument_model.bases['normRangeMin'][0] -\
-            external_instrument_model.bases['pwlRangeMin'][0] * scale
+        scale = ((external_instrument_model.bases['normRangeMax'] -
+                  external_instrument_model.bases['normRangeMin']) /
+                 (external_instrument_model.bases['pwlRangeMax'] -
+                  external_instrument_model.bases['pwlRangeMin']))
+        offset = (external_instrument_model.bases['normRangeMin'] -
+                  external_instrument_model.bases['pwlRangeMin'] * scale)
 
         sampling_pwl = external_instrument_model.wl_to_pwl(sampling)
         rescaled_pwl = (sampling_pwl * scale) + offset
 
-        bases_transformation = external_instrument_model.bases['transformationMatrix'][0]
-        evaluated_hermite_bases = np.array([_evaluate_hermite_function(n_h, pos, weight) for pos, weight in zip(
-            rescaled_pwl, weights) for n_h in np.arange(int(
-                external_instrument_model.bases['nInverseBasesCoefficients'][0]))]).reshape(
-                n_samples, int(external_instrument_model.bases['nInverseBasesCoefficients'][0]))
-        _design_matrix = external_instrument_model.bases['inverseBasesCoefficients'][0] @ evaluated_hermite_bases.T
+        bases_transformation = external_instrument_model.bases['transformationMatrix']
+        evaluated_hermite_bases = np.array([_evaluate_hermite_function(n_h, pos, weight) for pos, weight in
+                                            zip(rescaled_pwl, weights) for n_h in np.arange(
+                int(external_instrument_model.bases['nInverseBasesCoefficients']))]).reshape(
+            n_samples, int(external_instrument_model.bases['nInverseBasesCoefficients']))
+        _design_matrix = external_instrument_model.bases['inverseBasesCoefficients'] @ evaluated_hermite_bases.T
         transformed_design_matrix = bases_transformation @ _design_matrix
 
         hc = 1.e9 * nature.C * nature.PLANCK
 
         def compute_norm(wl):
             r = external_instrument_model.get_response(wl)
             if r > 0:
                 return hc / (satellite.TELESCOPE_PUPIL_AREA * r * wl)
             else:
                 return 0.0
 
         norm = np.array([compute_norm(wl) for wl in sampling])
         design_matrix = np.array([transformed_design_matrix[i] * norm for i in
-                                  np.arange(external_instrument_model.bases['nBases'][0])])
+                                  np.arange(external_instrument_model.bases['nBases'])])
 
         return cls(sampling, design_matrix=design_matrix)
 
     @classmethod
     def from_config(cls, sampling, bases_config):
         """
         Instantiate an object starting from a sampling grid and the configuration for the basis functions.
@@ -116,48 +117,66 @@
     def get_design_matrix(self):
         return self.design_matrix
 
     def get_sampling_grid(self):
         return self.sampling_grid
 
 
-def populate_design_matrix(sampling_grid, config):
-    """
-    Create a design matrix given the internal calibration bases and a user-defined sampling.
-
-    Args:
-        sampling_grid (ndarray): 1D array of positions where the bases need to be evaluated.
-        config (DataFrame): The configuration of the set of bases loaded into a DataFrame.
-
-    Returns:
-        ndarray: The resulting design matrix.
-    """
-    n_samples = len(sampling_grid)
-    scale = (config['normalizedRange'].iloc(0)[0][1] - config['normalizedRange'].iloc(0)[0][0]) /\
-            (config['range'].iloc(0)[0][1] - config['range'].iloc(0)[0][0])
-    offset = config['normalizedRange'].iloc(0)[0][0] - config['range'].iloc(0)[0][0] * scale
-    rescaled_pwl = (sampling_grid * scale) + offset
-
-    def psi(n, x): return 1.0 / np.sqrt(math.pow(2, n) * gamma(n + 1) *
-                                        np.sqrt(np.pi)) * np.exp(-x ** 2 / 2.0) * eval_hermite(n, x)
-
-    dimension = int(config['dimension'].iloc[0])
-    transformed_set_dimension = int(config['transformedSetDimension'].iloc[0])
-    bases_transformation = config['transformationMatrix'].iloc(0)[0].reshape(dimension, transformed_set_dimension)
-    design_matrix = np.array([psi(n_h, pos) for pos in rescaled_pwl for n_h in np.arange(dimension)]).reshape(n_samples,
-                                                                                                              dimension)
-    return bases_transformation @ design_matrix.T
-
-
 def _evaluate_hermite_function(n, x, w):
     return _hermite_function(n, x) if w > 0 else 0
 
 
 @functools.lru_cache(maxsize=128)
 def _hermite_function(n, x):
     if n == 0:
         return sqrt_4_pi * np.exp(-x ** 2. / 2.)
     elif n == 1:
         return sqrt_4_pi * np.exp(-x ** 2. / 2.) * np.sqrt(2.) * x
     c1 = np.sqrt(2. / n) * x
     c2 = -np.sqrt((n - 1) / n)
     return c1 * _hermite_function(n - 1, x) + c2 * _hermite_function(n - 2, x)
+
+
+def populate_design_matrix(sampling_grid, bases_config):
+    def __psi(n, x):
+        return (1.0 / np.sqrt(math.pow(2, n) * gamma(n + 1) * np.sqrt(np.pi)) * np.exp(-x ** 2 / 2.0) *
+                eval_hermite(n, x))
+
+    n_samples = len(sampling_grid)
+    bc_columns = bases_config.columns
+    if 'knots' not in bc_columns and 'transformedSetDimension' in bc_columns:  # Hermite
+        normalised_range_lower, normalised_range_upper = bases_config['normalizedRange'].iloc(0)[0]
+        range_lower, range_upper = bases_config['range'].iloc(0)[0]
+        scale = (normalised_range_upper - normalised_range_lower) / (range_upper - range_lower)
+        offset = normalised_range_lower - range_lower * scale
+        rescaled_pwl = (sampling_grid * scale) + offset
+        dimension = int(bases_config['dimension'].iloc[0])
+        transformed_set_dimension = int(bases_config['transformedSetDimension'].iloc[0])
+        bases_transformation = bases_config['transformationMatrix'].iloc(0)[0].reshape(dimension,
+                                                                                       transformed_set_dimension)
+        design_matrix = np.array([__psi(n_h, pos) for pos in rescaled_pwl for n_h in np.arange(dimension)]).reshape(
+            n_samples, dimension)
+        return bases_transformation @ design_matrix.T
+    elif 'knots' in bc_columns:  # Spline
+        if len(bases_config) != 1:
+            raise ValueError('Only one row should be accepted at a time.')
+        knots = bases_config['knots'].iloc[0]
+        n_knots = len(knots)
+        order = bases_config['order'].iloc[0]
+        degree = order - 1
+        n_bases = n_knots - order
+        if 'transformationMatrix' in bases_config.__dir__():
+            transformation_matrix = np.array(bases_config.transformationMatrix.values[0])
+            ts_dim = bases_config.transformedSetDimension.values[0]
+            bases_transformation = transformation_matrix.reshape(ts_dim, n_bases)
+        else:
+            bases_transformation = np.identity(n_bases)
+        design_matrix = np.zeros((n_bases, n_samples))
+
+        for basis_id in np.arange(n_bases):  # Evaluate
+            c = np.zeros(n_knots)
+            c[basis_id] = 1.0
+            basis = BSpline(knots, c, degree)
+            design_matrix[basis_id] = np.array([basis(pos) for pos in sampling_grid])
+        return bases_transformation.dot(design_matrix)
+    else:
+        raise ValueError('Design matrix cannot be populated from the given configuration.')
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/spectrum/sampled_spectrum.py` & `gaiaxpy-2.1.1/src/gaiaxpy/spectrum/sampled_spectrum.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,14 +103,17 @@
                 continuous representation.
             design_matrix (ndarray): 2D array containing the evaluation of the basis functions on the desired sampling
                 grid.
 
         Returns:
             ndarray: 1D array containing the flux values for all samples.
         """
+        if coefficients.shape[0] != 0 and coefficients.shape[0] != design_matrix.shape[0]:
+            raise ValueError("Coefficients length doesn't match the design matrix dimension. Please make sure you're "
+                             "using the correct input files and configuration.")
         if isinstance(coefficients, ndarray) and coefficients.size > 0:
             return coefficients @ design_matrix
         return nan
 
     @staticmethod
     def _sample_error(covariance, design_matrix, standard_deviation):
         """
@@ -124,17 +127,21 @@
             design_matrix (ndarray): 2D array containing the evaluation of the basis functions on the desired sampling
                 grid.
             standard_deviation (float): Standard deviation.
 
         Returns:
             ndarray: 1D array containing the errors in flux for all samples.
         """
-        if len(covariance) == 0:
-            return covariance
-        return np.sqrt(np.sum(np.multiply(design_matrix.T @ covariance, design_matrix.T), axis=1)) * standard_deviation
+        if isinstance(covariance, ndarray):
+            return np.sqrt(
+                np.sum(np.multiply(design_matrix.T @ covariance, design_matrix.T), axis=1)) * standard_deviation
+        elif np.isnan(covariance):
+            return float('NaN')
+        else:
+            raise TypeError('Covariance must be either a NumPy array or nan.')
 
     @staticmethod
     def _sample_covariance(covariance, design_matrix):
         """
         Given the covariance matrix and a design matrix containing the evaluation of each basis function at the
         positions corresponding to the samples, this method computes the covariance matrix of the sampled spectrum.
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/spectrum/single_synthetic_photometry.py` & `gaiaxpy-2.1.1/src/gaiaxpy/spectrum/single_synthetic_photometry.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,38 +4,21 @@
 Module to represent a synthetic photometry in a single photometric system.
 """
 
 import warnings
 
 import numpy as np
 
-from .absolute_sampled_spectrum import AbsoluteSampledSpectrum
+from .photometric_absolute_sampled_spectrum import PhotometricAbsoluteSampledSpectrum
 
 # Ignore negative flux, handled in the code.
 warnings.filterwarnings('ignore', category=RuntimeWarning)
 
 
-def flux_to_mag(flux, zero_point):
-    """
-    Convert flux to magnitude.
-
-    Args:
-        flux (float): Flux value.
-        zero_point (float): Photometric zero-point.
-
-    Returns:
-        float: The magnitude.
-    """
-    if flux <= 0:
-        return np.nan
-    result = -2.5 * np.log10(flux) + zero_point
-    return result
-
-
-class SingleSyntheticPhotometry(AbsoluteSampledSpectrum):
+class SingleSyntheticPhotometry(PhotometricAbsoluteSampledSpectrum):
     """
     Synthetic photometry derived from Gaia spectra in one photometric system.
     """
 
     def __init__(self, source_id, xp_spectra, sampled_bases, merge, photometric_system):
         """
         Initialise a synthetic photometry in a single photometric system.
@@ -45,25 +28,23 @@
             xp_spectra (dict): A dictionary containing the BP and RP continuous spectra.
             sampled_bases (dict): The set of basis functions sampled onto the grid defining the resolution of the final
                 sampled spectrum.
             merge (dict): The weighting factors for BP and RP sampled onto the grid defining the resolution of the final
                 sampled spectrum.
             photometric_system (PhotometricSystem): The photometric system of the synthetic photometry.
         """
-        AbsoluteSampledSpectrum.__init__(self, source_id, xp_spectra, sampled_bases, merge)
+        PhotometricAbsoluteSampledSpectrum.__init__(self, source_id, xp_spectra, sampled_bases, merge)
         self.photometric_system = photometric_system.value
         # Correct flux if necessary (regular Photometric systems return the original value)
-        flux = self.flux
-        self.flux = self.photometric_system._correct_flux(flux)
+        aux_flux = self.flux
+        self.flux = self.photometric_system._correct_flux(aux_flux)
         # Correct the errors
-        error = self.error
-        self.error = self.photometric_system._correct_error(flux, error)
+        self.error = self.photometric_system._correct_error(aux_flux, self.error)
         # Magnitude is computed from self.flux which is the corrected flux
-        self.mag = [flux_to_mag(flux, zero_point) for flux, zero_point in
-                    zip(self.flux, self.photometric_system.get_zero_points())]
+        self.mag = self._compute_mag()
 
     def _photometry_to_dict(self):
         """
         Represent the photometry as a dictionary.
 
         Returns:
             dict: A dictionary containing the source identifier and the synthetic photometry.
@@ -80,7 +61,27 @@
 
         Returns:
             dict: A dictionary containing a particular field of the synthetic photometry.
         """
         bands = self.photometric_system.get_bands()
         values = field
         return {f'{name}_{band}': values[i] for i, band in enumerate(bands)}
+
+    def _compute_mag(self):
+        def flux_to_mag(flux, zero_point):
+            """
+            Convert flux to magnitude.
+
+            Args:
+                flux (float): Flux value.
+                zero_point (float): Photometric zero-point.
+
+            Returns:
+                float: The magnitude.
+            """
+            if flux <= 0:
+                return np.nan
+            result = -2.5 * np.log10(flux) + zero_point
+            return result
+
+        return [flux_to_mag(flux, zero_point) for flux, zero_point in
+                zip(self.flux, self.photometric_system.get_zero_points())]
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/spectrum/utils.py` & `gaiaxpy-2.1.1/src/gaiaxpy/spectrum/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 import numpy as np
 import pandas as pd
 
 
 def get_covariance_matrix(row, band):
     columns = row.keys() if isinstance(row, dict) else row.index
     if f'{band}_covariance_matrix' in columns:
-        return row[f'{band}_covariance_matrix']
+        covariance_matrix = row[f'{band}_covariance_matrix']
+        return np.nan if covariance_matrix is None else covariance_matrix
     elif f'{band}_coefficient_covariances' in columns:
-        return row[f'{band}_coefficient_covariances']
+        coefficient_covariances = row[f'{band}_coefficient_covariances']
+        return np.nan if coefficient_covariances is None else coefficient_covariances
     elif f'{band}_coefficient_correlations' in columns:
         return _correlation_to_covariance_dr3int5(row[f'{band}_coefficient_correlations'],
                                                   row[f'{band}_coefficient_errors'],
                                                   row[f'{band}_standard_deviation'])
     raise ValueError(f'None of the expected columns could be found in the input row. Columns are: {columns}.')
 
 
@@ -30,15 +32,15 @@
         formal_errors (ndarray): Formal errors of the parameters.
         standard_deviation (float): Standard deviation of the LSQ solution.
 
     Returns:
         ndarray: The covariance matrix as a numpy array.
     """
     if pd.isna(standard_deviation):
-        return None
+        return np.nan
     diagonal_errors = np.diag(formal_errors) / standard_deviation
     return diagonal_errors @ correlation_matrix @ diagonal_errors
 
 
 def _correlation_to_covariance_dr3int4(correlation_matrix, formal_errors, standard_deviation):
     """
     Compute the covariance matrix from the correlation matrix and the parameter formal errors.
@@ -50,16 +52,15 @@
 
     Returns:
         ndarray: The covariance matrix as a numpy array.
     """
     diagonal_errors = np.diag(formal_errors) / standard_deviation
     correlation_matrix_aux = np.multiply(correlation_matrix, (standard_deviation * standard_deviation))
     np.fill_diagonal(correlation_matrix_aux, 1.)
-    covariance_matrix = diagonal_errors @ correlation_matrix_aux @ diagonal_errors
-    return covariance_matrix
+    return diagonal_errors @ correlation_matrix_aux @ diagonal_errors
 
 
 def _correlation_to_covariance_dr3int3(correlation_matrix, formal_errors):
     """
     Compute the covariance matrix from the correlation matrix and the parameter formal errors.
 
     Args:
@@ -75,14 +76,16 @@
     return covariance_matrix
 
 
 def _list_to_array(lst):
     """
     List to NumPy array.
     """
+    if lst is None or (isinstance(lst, float) and pd.isna(lst)):
+        return None
     if isinstance(lst, np.ndarray):
         return lst
     elif isinstance(lst, list):
         if not lst:
             raise ValueError('List cannot be empty.')
         else:
             return np.array(lst)
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/spectrum/xp_continuous_spectrum.py` & `gaiaxpy-2.1.1/src/gaiaxpy/spectrum/xp_continuous_spectrum.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 ====================================
 Module to represent a BP/RP continuous spectrum.
 """
 
 import numpy as np
 
 from gaiaxpy.core.generic_functions import array_to_symmetric_matrix
-from gaiaxpy.core.satellite import BANDS
 from .utils import _list_to_array, get_covariance_matrix
 from .xp_spectrum import XpSpectrum
 
 
 class XpContinuousSpectrum(XpSpectrum):
     """
     A Gaia BP/RP spectrum represented as a continuous function defined as the sum of a set of bases functions multiplied
@@ -31,15 +30,14 @@
             covariance (ndarray): 2D array containing the covariance of the least squares solution.
             standard_deviation (float): Standard deviation of the least squares solution.
         """
         XpSpectrum.__init__(self, source_id, xp)
         self.coefficients = coefficients
         self.covariance = covariance
         self.standard_deviation = standard_deviation
-        self.basis_function_id = {BANDS.bp: 56, BANDS.rp: 57}
 
     @classmethod
     def from_data_frame(cls, df, band):
         """
         Initialise XP continuous spectrum from a Pandas DataFrame.
 
         Args:
@@ -100,16 +98,15 @@
         return {
             'source_id': self.source_id,
             'xp': self.xp.upper(),
             'standard_deviation': self.standard_deviation,
             'coefficients': _list_to_array(self.coefficients),
             'coefficient_correlations': _list_to_array(_extract_lower_triangle(correlation_matrix)),
             'coefficient_errors': _list_to_array(diagonal),
-            'n_parameters': len(self.coefficients),
-            'basis_function_id': self.basis_function_id[self.xp]
+            'n_parameters': len(self.coefficients)
         }
 
 
 def _extract_lower_triangle(matrix):
     """
     Extract the lower triangle of the matrix without including the diagonal.
     """
```

### Comparing `GaiaXPy-2.1.0/gaiaxpy/spectrum/xp_sampled_spectrum.py` & `gaiaxpy-2.1.1/src/gaiaxpy/spectrum/xp_sampled_spectrum.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from numbers import Number
 
 import numpy as np
 
 from .sampled_spectrum import SampledSpectrum
 from .utils import _list_to_array
 from .xp_spectrum import XpSpectrum
-from ..core.generic_functions import correlation_from_covariance
+from ..core.generic_functions import correlation_from_covariance, is_array_empty, is_variable_empty
 
 
 class XpSampledSpectrum(XpSpectrum, SampledSpectrum):
     """
     A Gaia BP/RP spectrum sampled to a given grid of positions.
     """
 
     def __init__(self, source_id=0, xp=None, pos=None, flux=None, flux_error=None, cov=None, stdev=None):
         XpSpectrum.__init__(self, source_id, xp)
         self.pos = pos
-        self.n_samples = len(self.pos)
-        self.flux = flux
-        self.error = flux_error
-        self.stdev = stdev
-        self.covariance = cov
+        self.n_samples = None if is_array_empty(self.pos) else len(self.pos)
+        self.flux = None if is_array_empty(flux) else flux
+        self.error = None if is_array_empty(flux_error) else flux_error
+        self.stdev = None if is_variable_empty(stdev) else stdev
+        self.covariance = None if is_array_empty(cov) else cov
 
     @classmethod
     def from_data_frame(cls, df, sampling, band):
         """
         Initialise a sampled spectrum from a Pandas DataFrame.
 
         Args:
@@ -38,29 +38,14 @@
                 structure as used in the archive for the correlation matrix is expected.
             sampling (ndarray): Given sampling.
             band (str): Gaia photometer, can be either 'bp' or 'rp'.
         """
         return cls(df['source_id'], band, sampling, df['flux'], df['flux_error'], df['cov'])
 
     @classmethod
-    def from_sampled(cls, source_id, xp, pos, flux, flux_error, cov=None):
-        """
-        Initialise a spectrum.
-
-        Args:
-        source_id (long): The source identifier.
-        xp (object): The photometer enum (BP/RP).
-        pos (ndarray): The array of positions (in pseudo-wavelength or wavelength) of the samples.
-        flux (ndarray): The flux value of each sample.
-        flux_error (ndarray): The uncertainty on the flux value of each sample.
-        cov (ndarray): The covariance matrix.
-        """
-        return cls(source_id, xp, pos, flux, flux_error, cov)
-
-    @classmethod
     def from_continuous(cls, continuous_spectrum, sampled_basis_functions, truncation=-1, with_correlation=False):
         """
         Initialise a spectrum.
 
         Args:
             continuous_spectrum (XpContinuousSpectrum): The continuous representation of this spectrum.
             sampled_basis_functions (SampledBasisFunctions): The set of basis functions sampled onto the grid defining
@@ -71,45 +56,63 @@
                 the basis function set to preserve only the significant bases is optional. By default, no truncation
                 will be applied, i.e. all bases will be used.
             with_correlation (bool): Whether correlation information should be generated.
         """
         if continuous_spectrum and sampled_basis_functions:
             coefficients = continuous_spectrum.get_coefficients()
             design_matrix = sampled_basis_functions.get_design_matrix()
+            pos = sampled_basis_functions.get_sampling_grid()
+            if is_array_empty(coefficients):
+                return cls(continuous_spectrum.get_source_id(), continuous_spectrum.get_xp(), pos)
+            else:
+                covariance = continuous_spectrum.get_covariance()
+                if isinstance(truncation, Number) and truncation > 0:
+                    coefficients = coefficients[:truncation]
+                    covariance = covariance[:truncation, :truncation]
+                    design_matrix = design_matrix[:truncation][:]
+                stdev = continuous_spectrum.get_standard_deviation()
+                flux = SampledSpectrum._sample_flux(coefficients, design_matrix)
+                flux_error = SampledSpectrum._sample_error(covariance, design_matrix, stdev)
+                cov = SampledSpectrum._sample_covariance(covariance, design_matrix) if with_correlation else None
+                return cls(continuous_spectrum.get_source_id(), continuous_spectrum.get_xp(), pos, flux, flux_error,
+                           cov, stdev)
         else:
-            return None
-        covariance = continuous_spectrum.get_covariance()
+            raise ValueError('Either the continuous spectrum or the sampled basis functions argument is empty.')
 
-        if isinstance(truncation, Number) and truncation > 0:
-            coefficients = coefficients[:truncation]
-            covariance = covariance[:truncation, :truncation]
-            design_matrix = design_matrix[:truncation][:]
-
-        stdev = continuous_spectrum.get_standard_deviation()
-        pos = sampled_basis_functions.get_sampling_grid()
-        flux = SampledSpectrum._sample_flux(coefficients, design_matrix)
-        flux_error = SampledSpectrum._sample_error(covariance, design_matrix, stdev)
-        cov = SampledSpectrum._sample_covariance(covariance, design_matrix) if with_correlation else None
-        return cls(continuous_spectrum.get_source_id(), continuous_spectrum.get_xp(), pos, flux, flux_error, cov, stdev)
+    @classmethod
+    def from_sampled(cls, source_id, xp, pos, flux, flux_error, cov=None):
+        """
+        Initialise a spectrum.
+
+        Args:
+        source_id (long): The source identifier.
+        xp (object): The photometer enum (BP/RP).
+        pos (ndarray): The array of positions (in pseudo-wavelength or wavelength) of the samples.
+        flux (ndarray): The flux value of each sample.
+        flux_error (ndarray): The uncertainty on the flux value of each sample.
+        cov (ndarray): The covariance matrix.
+        """
+        return cls(source_id, xp, pos, flux, flux_error, cov)
 
-    def spectrum_to_dict(self):
+    def spectrum_to_dict(self, with_correlation):
         """
         Represent spectrum as dictionary.
 
         Returns:
             dict: A dictionary populated with the minimum set of parameters that need to be stored for this object. This
                 is optimised for writing large number of sampled spectra and for this reason the array of positions is
                 NOT included as it is expected to be the same for a batch of spectra. The array of positions can be
                 retrieved by calling the sampling_to_dict method.
         """
         spectrum_dict = {'source_id': self.source_id, 'xp': self.xp.upper(), 'flux': _list_to_array(self.flux),
                          'flux_error': _list_to_array(self.error)}
-        if self.covariance is not None:
+        if with_correlation:
             full_correlation = correlation_from_covariance(self.covariance)
-            spectrum_dict['correlation'] = full_correlation[np.tril_indices(full_correlation.shape[0], k=-1)]
+            spectrum_dict['correlation'] = full_correlation if \
+                full_correlation is None else full_correlation[np.tril_indices(full_correlation.shape[0], k=-1)]
             if self.stdev is not None:
                 spectrum_dict['standard_deviation'] = self.stdev
         return spectrum_dict
 
     def _sampling_to_dict(self):
         """
         Represent sampling as dictionary.
```

