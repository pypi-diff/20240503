# Comparing `tmp/bayesn-0.3.2.tar.gz` & `tmp/bayesn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesn-0.3.2.tar", last modified: Wed Mar 20 15:38:49 2024, max compression
+gzip compressed data, was "bayesn-0.4.0.tar", last modified: Fri May  3 17:08:51 2024, max compression
```

## Comparing `bayesn-0.3.2.tar` & `bayesn-0.4.0.tar`

### file list

```diff
@@ -1,173 +1,183 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.836287 bayesn-0.3.2/
--rw-r--r--   0 matt       (501) staff       (20)     1068 2023-09-26 15:34:24.000000 bayesn-0.3.2/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     1523 2024-01-16 00:31:35.000000 bayesn-0.3.2/MANIFEST.in
--rw-r--r--   0 matt       (501) staff       (20)     3528 2024-03-20 15:38:49.836220 bayesn-0.3.2/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     2689 2024-01-17 13:25:33.000000 bayesn-0.3.2/README.md
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.793950 bayesn-0.3.2/bayesn/
--rw-r--r--   0 matt       (501) staff       (20)       35 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/__init__.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.794694 bayesn-0.3.2/bayesn/bayesn-filters/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.790602 bayesn-0.3.2/bayesn/bayesn-filters/filters/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.789594 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.796845 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/
--rw-r--r--   0 matt       (501) staff       (20)     3452 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Bandicam.dat
--rw-r--r--   0 matt       (501) staff       (20)     8552 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/H_andi.txt
--rw-r--r--   0 matt       (501) staff       (20)     8681 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Handicam.dat
--rw-r--r--   0 matt       (501) staff       (20)     5252 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Iandicam.dat
--rw-r--r--   0 matt       (501) staff       (20)     4341 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/J_andi.txt
--rw-r--r--   0 matt       (501) staff       (20)     3779 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Jandicam.dat
--rw-r--r--   0 matt       (501) staff       (20)     6722 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Kandicam.dat
--rw-r--r--   0 matt       (501) staff       (20)       31 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/README
--rw-r--r--   0 matt       (501) staff       (20)     2050 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Randicam.dat
--rw-r--r--   0 matt       (501) staff       (20)     3327 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Vandicam.dat
--rw-r--r--   0 matt       (501) staff       (20)     7084 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Yandicam.dat
--rw-r--r--   0 matt       (501) staff       (20)      432 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/filters.dat
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.798063 bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/
--rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_g.txt
--rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_i.txt
--rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_r.txt
--rw-r--r--   0 matt       (501) staff       (20)    10514 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_u.txt
--rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_y.txt
--rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_z.txt
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.789760 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.798480 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.799569 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/IR/
--rw-r--r--   0 matt       (501) staff       (20)    11648 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/IR/F105W.dat
--rw-r--r--   0 matt       (501) staff       (20)    24400 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/IR/F125W.dat
--rw-r--r--   0 matt       (501) staff       (20)    16546 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/IR/F140W.dat
--rw-r--r--   0 matt       (501) staff       (20)    11834 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/IR/F160W.dat
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.802334 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/
--rw-r--r--   0 matt       (501) staff       (20)    36644 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F225W.dat
--rw-r--r--   0 matt       (501) staff       (20)    26993 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F275W.dat
--rw-r--r--   0 matt       (501) staff       (20)    69707 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F300X.dat
--rw-r--r--   0 matt       (501) staff       (20)    19704 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F336W.dat
--rw-r--r--   0 matt       (501) staff       (20)    33555 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F390W.dat
--rw-r--r--   0 matt       (501) staff       (20)    23742 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F438W.dat
--rw-r--r--   0 matt       (501) staff       (20)    41720 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F475W.dat
--rw-r--r--   0 matt       (501) staff       (20)    80285 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F555W.dat
--rw-r--r--   0 matt       (501) staff       (20)    44493 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F625W.dat
--rw-r--r--   0 matt       (501) staff       (20)    69196 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F814W.dat
--rw-r--r--   0 matt       (501) staff       (20)       57 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/filters.dat
--rw-r--r--   0 matt       (501) staff       (20)     4324 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/wfc3_ir_f160w.dat
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.790057 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.804451 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/
--rw-r--r--   0 matt       (501) staff       (20)    11237 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/D62_H_system_total.10
--rw-r--r--   0 matt       (501) staff       (20)     7066 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/D62_J_system_total.10
--rw-r--r--   0 matt       (501) staff       (20)    11551 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/D62_K_system_total.10
--rw-r--r--   0 matt       (501) staff       (20)    27053 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/H_DUP_TAM_scan_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)     6592 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/H_RetroCam_duPont_TAMU_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)    22000 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/J_DUP_TAM_scan_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)     5472 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/J_RetroCam_duPont_TAMU_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)    27571 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/K_DUP_TAM_scan_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)    12229 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/Y_DUP_TAM_scan_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)     4187 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/Y_RetroCam_duPont_TAMU_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)      814 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/filters.dat
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.808050 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/
--rw-r--r--   0 matt       (501) staff       (20)     5544 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/B_CSP2_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)     1904 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/B_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)    26697 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/H_SWO_TAM_scan_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)     8187 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/Jrc1_SWO_TAM_scan_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)    19250 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/Jrc2_SWO_TAM_scan_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)     2247 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/README
--rw-r--r--   0 matt       (501) staff       (20)     4179 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/V_CSP2_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)     2140 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/V_LC3009_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)     1920 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/V_LC3014_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)     1547 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/V_LC9844_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)    17700 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/Y_SWO_TAM_scan_atm.dat
--rw-r--r--   0 matt       (501) staff       (20)     2136 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/filters.dat
--rw-r--r--   0 matt       (501) staff       (20)     4242 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/g_CSP2_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)     1717 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/g_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)     4290 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/i_CSP2_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)     1919 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/i_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)    12675 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/kfilter
--rw-r--r--   0 matt       (501) staff       (20)     4532 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/r_CSP2_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)     3711 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/r_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)     2310 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/u_CSP2_tel_ccd_atm_ext_1.2.dat
--rw-r--r--   0 matt       (501) staff       (20)      867 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/u_tel_ccd_atm_ext_1.2.dat
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.816697 bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/
--rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_g.dat
--rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_i.dat
--rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_r.dat
--rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_u.dat
--rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_y.dat
--rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_z.dat
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.818076 bayesn-0.3.2/bayesn/bayesn-filters/filters/NULL/
--rw-r--r--   0 matt       (501) staff       (20)     7830 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/NULL/NULL.dat
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.819157 bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/
--rw-r--r--   0 matt       (501) staff       (20)     9351 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/g_filt_revised.txt
--rw-r--r--   0 matt       (501) staff       (20)     5427 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/g_filt_tonry.txt
--rw-r--r--   0 matt       (501) staff       (20)     5427 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/i_filt_tonry.txt
--rw-r--r--   0 matt       (501) staff       (20)     5427 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/r_filt_tonry.txt
--rw-r--r--   0 matt       (501) staff       (20)     5697 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/y_filt_tonry.txt
--rw-r--r--   0 matt       (501) staff       (20)     5427 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/z_filt_tonry.txt
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.790368 bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.820453 bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/
--rw-r--r--   0 matt       (501) staff       (20)      318 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/filters.dat
--rw-r--r--   0 matt       (501) staff       (20)     2288 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonB_UVOT.dat
--rw-r--r--   0 matt       (501) staff       (20)     8046 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVM2.dat
--rw-r--r--   0 matt       (501) staff       (20)    14499 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVW1.dat
--rw-r--r--   0 matt       (501) staff       (20)    17307 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVW2.dat
--rw-r--r--   0 matt       (501) staff       (20)     2658 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonU_UVOT.dat
--rw-r--r--   0 matt       (501) staff       (20)     3443 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonV_UVOT.dat
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.790477 bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.821251 bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/
--rw-r--r--   0 matt       (501) staff       (20)      326 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/filters.dat
--rw-r--r--   0 matt       (501) staff       (20)      879 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_g.res
--rw-r--r--   0 matt       (501) staff       (20)      978 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_i.res
--rw-r--r--   0 matt       (501) staff       (20)      900 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_r.res
--rw-r--r--   0 matt       (501) staff       (20)      916 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_u.res
--rw-r--r--   0 matt       (501) staff       (20)     1122 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_z.res
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.822070 bayesn-0.3.2/bayesn/bayesn-filters/filters/ZTF/
--rw-r--r--   0 matt       (501) staff       (20)    96650 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/ZTF/p48g.txt
--rw-r--r--   0 matt       (501) staff       (20)    52300 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/ZTF/p48i.txt
--rw-r--r--   0 matt       (501) staff       (20)   160050 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/ZTF/p48r.txt
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.790765 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.823205 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/
--rw-r--r--   0 matt       (501) staff       (20)     1218 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_H.dat
--rw-r--r--   0 matt       (501) staff       (20)     2247 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_J.dat
--rw-r--r--   0 matt       (501) staff       (20)     1596 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_Ks.dat
--rw-r--r--   0 matt       (501) staff       (20)      371 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/filters.dat
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.824055 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/
--rw-r--r--   0 matt       (501) staff       (20)      129 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/filters.dat
--rw-r--r--   0 matt       (501) staff       (20)     8865 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/hfilter
--rw-r--r--   0 matt       (501) staff       (20)     6910 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/jfilter
--rw-r--r--   0 matt       (501) staff       (20)    12675 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/kfilter
--rw-r--r--   0 matt       (501) staff       (20)     5202 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/yfilter
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.825181 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/stritzinger/
--rw-r--r--   0 matt       (501) staff       (20)      320 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/stritzinger/b_stritzinger
--rw-r--r--   0 matt       (501) staff       (20)      400 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/stritzinger/filters.dat
--rw-r--r--   0 matt       (501) staff       (20)     3978 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/stritzinger/i_stritzinger
--rw-r--r--   0 matt       (501) staff       (20)     6322 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/stritzinger/r_stritzinger
--rw-r--r--   0 matt       (501) staff       (20)      400 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/stritzinger/u_stritzinger
--rw-r--r--   0 matt       (501) staff       (20)      384 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/stritzinger/v_stritzinger
--rw-r--r--   0 matt       (501) staff       (20)     7196 2024-03-20 15:34:44.000000 bayesn-0.3.2/bayesn/bayesn-filters/filters.yaml
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.826244 bayesn-0.3.2/bayesn/bayesn-filters/standards/
--rw-r--r--   0 matt       (501) staff       (20)   288000 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/standards/alpha_lyr_stis_010.fits
--rw-r--r--   0 matt       (501) staff       (20)    66710 2024-01-16 00:31:35.000000 bayesn-0.3.2/bayesn/bayesn-filters/standards/bd_17d4708_stisnic_007.dat
--rw-r--r--   0 matt       (501) staff       (20)     5281 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/bayesn_io.py
--rw-r--r--   0 matt       (501) staff       (20)   141575 2024-03-20 15:34:44.000000 bayesn-0.3.2/bayesn/bayesn_model.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.826883 bayesn-0.3.2/bayesn/data/
--rw-r--r--   0 matt       (501) staff       (20)  2042248 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/data/hsiao.h5
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.829805 bayesn-0.3.2/bayesn/model_files/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.834471 bayesn-0.3.2/bayesn/model_files/M20_model/
--rw-r--r--   0 matt       (501) staff       (20)     1197 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/model_files/M20_model/BAYESN.INFO
--rw-r--r--   0 matt       (501) staff       (20)    14342 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/model_files/M20_model/BAYESN.YAML
--rw-r--r--   0 matt       (501) staff       (20)     5020 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/model_files/README.md
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.834797 bayesn-0.3.2/bayesn/model_files/T21_model/
--rw-r--r--   0 matt       (501) staff       (20)     1088 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/model_files/T21_model/BAYESN.INFO
--rw-r--r--   0 matt       (501) staff       (20)     5174 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/model_files/T21_model/BAYESN.YAML
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.835102 bayesn-0.3.2/bayesn/model_files/W22_model/
--rw-r--r--   0 matt       (501) staff       (20)     1124 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/model_files/W22_model/BAYESN.INFO
--rw-r--r--   0 matt       (501) staff       (20)    23104 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/model_files/W22_model/BAYESN.YAML
--rw-r--r--   0 matt       (501) staff       (20)     4494 2023-09-26 15:34:24.000000 bayesn-0.3.2/bayesn/spline_utils.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.835584 bayesn-0.3.2/bayesn.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     3528 2024-03-20 15:38:49.000000 bayesn-0.3.2/bayesn.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     7112 2024-03-20 15:38:49.000000 bayesn-0.3.2/bayesn.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2024-03-20 15:38:49.000000 bayesn-0.3.2/bayesn.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)      151 2024-03-20 15:38:49.000000 bayesn-0.3.2/bayesn.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)       17 2024-03-20 15:38:49.000000 bayesn-0.3.2/bayesn.egg-info/top_level.txt
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-03-20 15:38:49.835288 bayesn-0.3.2/docs/
--rw-r--r--   0 matt       (501) staff       (20)     1189 2024-03-20 15:34:44.000000 bayesn-0.3.2/docs/conf.py
--rw-r--r--   0 matt       (501) staff       (20)      100 2023-09-26 15:34:24.000000 bayesn-0.3.2/pyproject.toml
--rwxr-xr-x   0 matt       (501) staff       (20)     2379 2024-01-16 00:31:35.000000 bayesn-0.3.2/run_bayesn
--rw-r--r--   0 matt       (501) staff       (20)     1870 2024-03-20 15:38:49.836608 bayesn-0.3.2/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)       38 2023-09-26 15:34:24.000000 bayesn-0.3.2/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.071225 bayesn-0.4.0/
+-rw-r--r--   0 matt       (501) staff       (20)     1068 2023-09-26 15:34:24.000000 bayesn-0.4.0/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     1610 2024-05-02 15:16:20.000000 bayesn-0.4.0/MANIFEST.in
+-rw-r--r--   0 matt       (501) staff       (20)     3576 2024-05-03 17:08:51.071157 bayesn-0.4.0/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     2737 2024-05-03 17:07:45.000000 bayesn-0.4.0/README.md
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.048412 bayesn-0.4.0/bayesn/
+-rw-r--r--   0 matt       (501) staff       (20)       35 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/__init__.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.049297 bayesn-0.4.0/bayesn/bayesn-filters/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.045808 bayesn-0.4.0/bayesn/bayesn-filters/filters/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.044650 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.050757 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/
+-rw-r--r--   0 matt       (501) staff       (20)     3452 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Bandicam.dat
+-rw-r--r--   0 matt       (501) staff       (20)     8552 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/H_andi.txt
+-rw-r--r--   0 matt       (501) staff       (20)     8681 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Handicam.dat
+-rw-r--r--   0 matt       (501) staff       (20)     5252 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Iandicam.dat
+-rw-r--r--   0 matt       (501) staff       (20)     4341 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/J_andi.txt
+-rw-r--r--   0 matt       (501) staff       (20)     3779 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Jandicam.dat
+-rw-r--r--   0 matt       (501) staff       (20)     6722 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Kandicam.dat
+-rw-r--r--   0 matt       (501) staff       (20)       31 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/README
+-rw-r--r--   0 matt       (501) staff       (20)     2050 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Randicam.dat
+-rw-r--r--   0 matt       (501) staff       (20)     3327 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Vandicam.dat
+-rw-r--r--   0 matt       (501) staff       (20)     7084 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Yandicam.dat
+-rw-r--r--   0 matt       (501) staff       (20)      432 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/filters.dat
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.052007 bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/
+-rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_g.txt
+-rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_i.txt
+-rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_r.txt
+-rw-r--r--   0 matt       (501) staff       (20)    10514 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_u.txt
+-rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_y.txt
+-rw-r--r--   0 matt       (501) staff       (20)    21816 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_z.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.044826 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.052332 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.052966 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/IR/
+-rw-r--r--   0 matt       (501) staff       (20)    11648 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/IR/F105W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    24400 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/IR/F125W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    16546 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/IR/F140W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    11834 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/IR/F160W.dat
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.055492 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/
+-rw-r--r--   0 matt       (501) staff       (20)    36644 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F225W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    26993 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F275W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    69707 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F300X.dat
+-rw-r--r--   0 matt       (501) staff       (20)    19704 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F336W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    33555 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F390W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    23742 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F438W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    41720 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F475W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    80285 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F555W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    44493 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F625W.dat
+-rw-r--r--   0 matt       (501) staff       (20)    69196 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F814W.dat
+-rw-r--r--   0 matt       (501) staff       (20)       57 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/filters.dat
+-rw-r--r--   0 matt       (501) staff       (20)     4324 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/wfc3_ir_f160w.dat
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.045117 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.056982 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/
+-rw-r--r--   0 matt       (501) staff       (20)    11237 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/D62_H_system_total.10
+-rw-r--r--   0 matt       (501) staff       (20)     7066 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/D62_J_system_total.10
+-rw-r--r--   0 matt       (501) staff       (20)    11551 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/D62_K_system_total.10
+-rw-r--r--   0 matt       (501) staff       (20)    27053 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/H_DUP_TAM_scan_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)     6592 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/H_RetroCam_duPont_TAMU_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)    22000 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/J_DUP_TAM_scan_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)     5472 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/J_RetroCam_duPont_TAMU_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)    27571 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/K_DUP_TAM_scan_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)    12229 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/Y_DUP_TAM_scan_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)     4187 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/Y_RetroCam_duPont_TAMU_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)      814 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/filters.dat
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.059854 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/
+-rw-r--r--   0 matt       (501) staff       (20)     5544 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/B_CSP2_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     1904 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/B_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)    26697 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/H_SWO_TAM_scan_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)     8187 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/Jrc1_SWO_TAM_scan_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)    19250 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/Jrc2_SWO_TAM_scan_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)     2247 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/README
+-rw-r--r--   0 matt       (501) staff       (20)     4179 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/V_CSP2_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     2140 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/V_LC3009_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     1920 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/V_LC3014_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     1547 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/V_LC9844_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)    17700 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/Y_SWO_TAM_scan_atm.dat
+-rw-r--r--   0 matt       (501) staff       (20)     2136 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/filters.dat
+-rw-r--r--   0 matt       (501) staff       (20)     4242 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/g_CSP2_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     1717 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/g_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     4290 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/i_CSP2_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     1919 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/i_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)    12675 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/kfilter
+-rw-r--r--   0 matt       (501) staff       (20)     4532 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/r_CSP2_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     3711 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/r_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     2310 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/u_CSP2_tel_ccd_atm_ext_1.2.dat
+-rw-r--r--   0 matt       (501) staff       (20)      867 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/u_tel_ccd_atm_ext_1.2.dat
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.061699 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.062769 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/2017-04_approx/
+-rw-r--r--   0 matt       (501) staff       (20)    39688 2024-03-20 15:34:44.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_g.dat
+-rw-r--r--   0 matt       (501) staff       (20)    34496 2024-03-20 15:34:44.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_i.dat
+-rw-r--r--   0 matt       (501) staff       (20)    37136 2024-03-20 15:34:44.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_r.dat
+-rw-r--r--   0 matt       (501) staff       (20)    22660 2024-03-20 15:34:44.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_u.dat
+-rw-r--r--   0 matt       (501) staff       (20)    42020 2024-03-20 15:34:44.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_y.dat
+-rw-r--r--   0 matt       (501) staff       (20)    29788 2024-03-20 15:34:44.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_z.dat
+-rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_g.dat
+-rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_i.dat
+-rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_r.dat
+-rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_u.dat
+-rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_y.dat
+-rw-r--r--   0 matt       (501) staff       (20)   389500 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_z.dat
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.062908 bayesn-0.4.0/bayesn/bayesn-filters/filters/NULL/
+-rw-r--r--   0 matt       (501) staff       (20)     7830 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/NULL/NULL.dat
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.063823 bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/
+-rw-r--r--   0 matt       (501) staff       (20)     9351 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/g_filt_revised.txt
+-rw-r--r--   0 matt       (501) staff       (20)     5427 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/g_filt_tonry.txt
+-rw-r--r--   0 matt       (501) staff       (20)     5427 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/i_filt_tonry.txt
+-rw-r--r--   0 matt       (501) staff       (20)     5427 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/r_filt_tonry.txt
+-rw-r--r--   0 matt       (501) staff       (20)     5697 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/y_filt_tonry.txt
+-rw-r--r--   0 matt       (501) staff       (20)     5427 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/z_filt_tonry.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.045513 bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.064796 bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/
+-rw-r--r--   0 matt       (501) staff       (20)      318 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/filters.dat
+-rw-r--r--   0 matt       (501) staff       (20)     2288 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonB_UVOT.dat
+-rw-r--r--   0 matt       (501) staff       (20)     8046 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVM2.dat
+-rw-r--r--   0 matt       (501) staff       (20)    14499 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVW1.dat
+-rw-r--r--   0 matt       (501) staff       (20)    17307 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVW2.dat
+-rw-r--r--   0 matt       (501) staff       (20)     2658 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonU_UVOT.dat
+-rw-r--r--   0 matt       (501) staff       (20)     3443 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonV_UVOT.dat
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.045647 bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.065474 bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/
+-rw-r--r--   0 matt       (501) staff       (20)      326 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/filters.dat
+-rw-r--r--   0 matt       (501) staff       (20)      879 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_g.res
+-rw-r--r--   0 matt       (501) staff       (20)      978 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_i.res
+-rw-r--r--   0 matt       (501) staff       (20)      900 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_r.res
+-rw-r--r--   0 matt       (501) staff       (20)      916 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_u.res
+-rw-r--r--   0 matt       (501) staff       (20)     1122 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_z.res
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.065909 bayesn-0.4.0/bayesn/bayesn-filters/filters/ZTF/
+-rw-r--r--   0 matt       (501) staff       (20)    96650 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/ZTF/p48g.txt
+-rw-r--r--   0 matt       (501) staff       (20)    52300 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/ZTF/p48i.txt
+-rw-r--r--   0 matt       (501) staff       (20)   160050 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/ZTF/p48r.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.046018 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.066465 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/
+-rw-r--r--   0 matt       (501) staff       (20)     1218 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_H.dat
+-rw-r--r--   0 matt       (501) staff       (20)     2247 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_J.dat
+-rw-r--r--   0 matt       (501) staff       (20)     1596 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_Ks.dat
+-rw-r--r--   0 matt       (501) staff       (20)      371 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/filters.dat
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.067022 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/
+-rw-r--r--   0 matt       (501) staff       (20)      129 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/filters.dat
+-rw-r--r--   0 matt       (501) staff       (20)     8865 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/hfilter
+-rw-r--r--   0 matt       (501) staff       (20)     6910 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/jfilter
+-rw-r--r--   0 matt       (501) staff       (20)    12675 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/kfilter
+-rw-r--r--   0 matt       (501) staff       (20)     5202 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/yfilter
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.067656 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/stritzinger/
+-rw-r--r--   0 matt       (501) staff       (20)      320 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/stritzinger/b_stritzinger
+-rw-r--r--   0 matt       (501) staff       (20)      400 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/stritzinger/filters.dat
+-rw-r--r--   0 matt       (501) staff       (20)     3978 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/stritzinger/i_stritzinger
+-rw-r--r--   0 matt       (501) staff       (20)     6322 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/stritzinger/r_stritzinger
+-rw-r--r--   0 matt       (501) staff       (20)      400 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/stritzinger/u_stritzinger
+-rw-r--r--   0 matt       (501) staff       (20)      384 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/stritzinger/v_stritzinger
+-rw-r--r--   0 matt       (501) staff       (20)     7856 2024-04-29 13:21:40.000000 bayesn-0.4.0/bayesn/bayesn-filters/filters.yaml
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.068056 bayesn-0.4.0/bayesn/bayesn-filters/standards/
+-rw-r--r--   0 matt       (501) staff       (20)   288000 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/standards/alpha_lyr_stis_010.fits
+-rw-r--r--   0 matt       (501) staff       (20)    66710 2024-01-16 00:31:35.000000 bayesn-0.4.0/bayesn/bayesn-filters/standards/bd_17d4708_stisnic_007.dat
+-rw-r--r--   0 matt       (501) staff       (20)     5281 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/bayesn_io.py
+-rw-r--r--   0 matt       (501) staff       (20)   170739 2024-05-03 17:07:45.000000 bayesn-0.4.0/bayesn/bayesn_model.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.068214 bayesn-0.4.0/bayesn/data/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.069410 bayesn-0.4.0/bayesn/data/example_lcs/
+-rw-r--r--   0 matt       (501) staff       (20)     3004 2024-05-02 15:16:20.000000 bayesn-0.4.0/bayesn/data/example_lcs/Foundation_DR1_2016W.txt
+-rw-r--r--   0 matt       (501) staff       (20)  2042248 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/data/hsiao.h5
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.069529 bayesn-0.4.0/bayesn/model_files/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.069772 bayesn-0.4.0/bayesn/model_files/M20_model/
+-rw-r--r--   0 matt       (501) staff       (20)     1197 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/model_files/M20_model/BAYESN.INFO
+-rw-r--r--   0 matt       (501) staff       (20)    14342 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/model_files/M20_model/BAYESN.YAML
+-rw-r--r--   0 matt       (501) staff       (20)     5020 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/model_files/README.md
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.070001 bayesn-0.4.0/bayesn/model_files/T21_model/
+-rw-r--r--   0 matt       (501) staff       (20)     1088 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/model_files/T21_model/BAYESN.INFO
+-rw-r--r--   0 matt       (501) staff       (20)     5174 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/model_files/T21_model/BAYESN.YAML
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.070220 bayesn-0.4.0/bayesn/model_files/W22_model/
+-rw-r--r--   0 matt       (501) staff       (20)     1124 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/model_files/W22_model/BAYESN.INFO
+-rw-r--r--   0 matt       (501) staff       (20)    23104 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/model_files/W22_model/BAYESN.YAML
+-rw-r--r--   0 matt       (501) staff       (20)     4494 2023-09-26 15:34:24.000000 bayesn-0.4.0/bayesn/spline_utils.py
+-rw-r--r--   0 matt       (501) staff       (20)     9125 2024-05-02 09:05:21.000000 bayesn-0.4.0/bayesn/zltn_utils.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.070524 bayesn-0.4.0/bayesn.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     3576 2024-05-03 17:08:51.000000 bayesn-0.4.0/bayesn.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     7548 2024-05-03 17:08:51.000000 bayesn-0.4.0/bayesn.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2024-05-03 17:08:51.000000 bayesn-0.4.0/bayesn.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)      151 2024-05-03 17:08:51.000000 bayesn-0.4.0/bayesn.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)       23 2024-05-03 17:08:51.000000 bayesn-0.4.0/bayesn.egg-info/top_level.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-05-03 17:08:51.070357 bayesn-0.4.0/docs/
+-rw-r--r--   0 matt       (501) staff       (20)     1189 2024-05-03 17:07:45.000000 bayesn-0.4.0/docs/conf.py
+-rw-r--r--   0 matt       (501) staff       (20)      100 2023-09-26 15:34:24.000000 bayesn-0.4.0/pyproject.toml
+-rwxr-xr-x   0 matt       (501) staff       (20)     2441 2024-05-02 09:05:21.000000 bayesn-0.4.0/run_bayesn
+-rw-r--r--   0 matt       (501) staff       (20)     1943 2024-05-03 17:08:51.071544 bayesn-0.4.0/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)       38 2023-09-26 15:34:24.000000 bayesn-0.4.0/setup.py
```

### Comparing `bayesn-0.3.2/LICENSE` & `bayesn-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/MANIFEST.in` & `bayesn-0.4.0/MANIFEST.in`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-include bayesn/data/hsiao.h5
+include bayesn/data/*
+include bayesn/data/example_lcs/*
 include bayesn/bayesn-filters/*
 include bayesn/bayesn-filters/filters/*
 include bayesn/bayesn-filters/filters/CTIO/*
 include bayesn/bayesn-filters/filters/CTIO/ANDICAM/*
 include bayesn/bayesn-filters/filters/DECam/*
 include bayesn/bayesn-filters/filters/HST/WFC3/*
 include bayesn/bayesn-filters/filters/HST/WFC3/IR/*
 include bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/*
 include bayesn/bayesn-filters/filters/LCO/*
 include bayesn/bayesn-filters/filters/LCO/Dupont/*
 include bayesn/bayesn-filters/filters/LCO/Swope/*
 include bayesn/bayesn-filters/filters/LSST/*
+include bayesn/bayesn-filters/filters/LSST/2017-04_approx/*
 include bayesn/bayesn-filters/filters/NULL/*
 include bayesn/bayesn-filters/filters/PS1/*
 include bayesn/bayesn-filters/filters/standard/*
 include bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/*
 include bayesn/bayesn-filters/filters/standard/Persson/*
 include bayesn/bayesn-filters/filters/standard/stritzinger/*
 include bayesn/bayesn-filters/filters/Swift/*
```

### Comparing `bayesn-0.3.2/PKG-INFO` & `bayesn-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesn
-Version: 0.3.2
+Version: 0.4.0
 Summary: Hierarchical Bayesian modelling of type Ia SNe
 Home-page: https://github.com/bayesn/bayesn
 Author: Matt Grayling, Stephen Thorp, Kaisey Mandel
 Author-email: mg2102@cam.ac.uk
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,15 +35,15 @@
 Developed and maintained by: Matt Grayling (@mattgrayling), Stephen Thorp (@stevet40), Gautham Narayan (@gnarayan), and 
 Kaisey S. Mandel (@CambridgeAstroStat) on behalf of the BayeSN Team (@bayesn).
 
 ## About
 BayeSN is a probabilistic optical-NIR SED model for type Ia supernovae, allowing for hierarchical analysis of the
 population distribution of physical properties as well as cosmology-independent distance estimation for individual
 SNe. This repository contains an implementation of the BayeSN SED model built with numpyro and jax, with support for 
-GPU acceleration, as discussed in Grayling+2024 (submitted to MNRAS).
+GPU acceleration, as discussed in Grayling+2024 (`arXiv link <https://arxiv.org/abs/2401.08755>`, accepted by MNRAS).
 
 ## Installation and usage
 BayeSN can be pip-installed via the command `pip install bayesn`. 
 
 Detailed instructions on how to install and run the BayeSN model can be found here: https://bayesn.readthedocs.io/en/latest/index.html
 
 ## Support
```

### Comparing `bayesn-0.3.2/README.md` & `bayesn-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Developed and maintained by: Matt Grayling (@mattgrayling), Stephen Thorp (@stevet40), Gautham Narayan (@gnarayan), and 
 Kaisey S. Mandel (@CambridgeAstroStat) on behalf of the BayeSN Team (@bayesn).
 
 ## About
 BayeSN is a probabilistic optical-NIR SED model for type Ia supernovae, allowing for hierarchical analysis of the
 population distribution of physical properties as well as cosmology-independent distance estimation for individual
 SNe. This repository contains an implementation of the BayeSN SED model built with numpyro and jax, with support for 
-GPU acceleration, as discussed in Grayling+2024 (submitted to MNRAS).
+GPU acceleration, as discussed in Grayling+2024 (`arXiv link <https://arxiv.org/abs/2401.08755>`, accepted by MNRAS).
 
 ## Installation and usage
 BayeSN can be pip-installed via the command `pip install bayesn`. 
 
 Detailed instructions on how to install and run the BayeSN model can be found here: https://bayesn.readthedocs.io/en/latest/index.html
 
 ## Support
```

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Bandicam.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Bandicam.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/H_andi.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/H_andi.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Handicam.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Handicam.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Iandicam.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Iandicam.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/J_andi.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/J_andi.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Jandicam.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Jandicam.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Kandicam.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Kandicam.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Randicam.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Randicam.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Vandicam.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Vandicam.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Yandicam.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/CTIO/ANDICAM/Yandicam.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_g.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_g.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_i.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_i.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_r.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_r.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_u.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_u.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_y.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_y.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/DECam/decam_z.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/DECam/decam_z.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/IR/F105W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/IR/F105W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/IR/F125W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/IR/F125W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/IR/F140W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/IR/F140W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/IR/F160W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/IR/F160W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F225W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F225W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F275W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F275W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F300X.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F300X.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F336W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F336W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F390W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F390W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F438W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F438W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F475W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F475W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F555W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F555W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F625W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F625W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F814W.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/F814W.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/HST/WFC3/wfc3_ir_f160w.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/HST/WFC3/wfc3_ir_f160w.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/D62_H_system_total.10` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/D62_H_system_total.10`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/D62_J_system_total.10` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/D62_J_system_total.10`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/D62_K_system_total.10` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/D62_K_system_total.10`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/H_DUP_TAM_scan_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/H_DUP_TAM_scan_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/H_RetroCam_duPont_TAMU_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/H_RetroCam_duPont_TAMU_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/J_DUP_TAM_scan_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/J_DUP_TAM_scan_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/J_RetroCam_duPont_TAMU_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/J_RetroCam_duPont_TAMU_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/K_DUP_TAM_scan_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/K_DUP_TAM_scan_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/Y_DUP_TAM_scan_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/Y_DUP_TAM_scan_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/Y_RetroCam_duPont_TAMU_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/Y_RetroCam_duPont_TAMU_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Dupont/filters.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Dupont/filters.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/B_CSP2_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/B_CSP2_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/B_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/B_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/H_SWO_TAM_scan_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/H_SWO_TAM_scan_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/Jrc1_SWO_TAM_scan_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/Jrc1_SWO_TAM_scan_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/Jrc2_SWO_TAM_scan_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/Jrc2_SWO_TAM_scan_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/README` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/README`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/V_CSP2_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/V_CSP2_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/V_LC3009_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/V_LC3009_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/V_LC3014_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/V_LC3014_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/V_LC9844_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/V_LC9844_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/Y_SWO_TAM_scan_atm.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/Y_SWO_TAM_scan_atm.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/filters.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/filters.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/g_CSP2_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/g_CSP2_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/g_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/g_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/i_CSP2_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/i_CSP2_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/i_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/i_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/kfilter` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/kfilter`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/r_CSP2_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/r_CSP2_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/r_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/r_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/u_CSP2_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/u_CSP2_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LCO/Swope/u_tel_ccd_atm_ext_1.2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LCO/Swope/u_tel_ccd_atm_ext_1.2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_g.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_g.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_i.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_i.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_r.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_r.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_u.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_u.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_y.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_y.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/LSST/total_z.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/LSST/total_z.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/NULL/NULL.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/NULL/NULL.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/g_filt_revised.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/g_filt_revised.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/g_filt_tonry.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/g_filt_tonry.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/i_filt_tonry.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/i_filt_tonry.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/r_filt_tonry.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/r_filt_tonry.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/y_filt_tonry.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/y_filt_tonry.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/PS1/z_filt_tonry.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/PS1/z_filt_tonry.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonB_UVOT.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonB_UVOT.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVM2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVM2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVW1.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVW1.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVW2.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonUVW2.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonU_UVOT.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonU_UVOT.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/Swift/UVOT/photonV_UVOT.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/Swift/UVOT/photonV_UVOT.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_g.res` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_g.res`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_i.res` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_i.res`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_r.res` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_r.res`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_u.res` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_u.res`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/USNO/USNO40/usno_z.res` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/USNO/USNO40/usno_z.res`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/ZTF/p48g.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/ZTF/p48g.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/ZTF/p48i.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/ZTF/p48i.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/ZTF/p48r.txt` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/ZTF/p48r.txt`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_H.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_H.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_J.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_J.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_Ks.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_Ks.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/hfilter` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/hfilter`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/jfilter` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/jfilter`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/kfilter` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/kfilter`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/Persson/yfilter` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/Persson/yfilter`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/stritzinger/i_stritzinger` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/stritzinger/i_stritzinger`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters/standard/stritzinger/r_stritzinger` & `bayesn-0.4.0/bayesn/bayesn-filters/filters/standard/stritzinger/r_stritzinger`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/filters.yaml` & `bayesn-0.4.0/bayesn/bayesn-filters/filters.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,352 +1,350 @@
-standards_root: standards
 standards:
   vega:
-    path: alpha_lyr_stis_010.fits
+    path: standards/alpha_lyr_stis_010.fits
   bd17:
-    path: bd_17d4708_stisnic_007.dat
-filters_root: filters
+    path: standards/bd_17d4708_stisnic_007.dat
 filters:
   B:
     magsys: vega
     magzero: 0.0
-    path: standard/stritzinger/b_stritzinger
+    path: filters/standard/stritzinger/b_stritzinger
   B_CSP:
     magsys: bd17
     magzero: 9.896
-    path: LCO/Swope/B_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/B_tel_ccd_atm_ext_1.2.dat
   B_CSP2:
     magsys: vega
     magzero: 0.03
-    path: LCO/Swope/B_CSP2_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/B_CSP2_tel_ccd_atm_ext_1.2.dat
   B_SWIFT:
     magsys: vega
     magzero: 0.0
-    path: Swift/UVOT/photonB_UVOT.dat
+    path: filters/Swift/UVOT/photonB_UVOT.dat
   F105W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/IR/F105W.dat
+    path: filters/HST/WFC3/IR/F105W.dat
   F125W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/IR/F125W.dat
+    path: filters/HST/WFC3/IR/F125W.dat
   F140W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/IR/F140W.dat
+    path: filters/HST/WFC3/IR/F140W.dat
   F160W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/IR/F160W.dat
+    path: filters/HST/WFC3/IR/F160W.dat
   F225W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F225W.dat
+    path: filters/HST/WFC3/UVIS2/F225W.dat
   F275W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F275W.dat
+    path: filters/HST/WFC3/UVIS2/F275W.dat
   F300X:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F300X.dat
+    path: filters/HST/WFC3/UVIS2/F300X.dat
   F336W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F336W.dat
+    path: filters/HST/WFC3/UVIS2/F336W.dat
   F390W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F390W.dat
+    path: filters/HST/WFC3/UVIS2/F390W.dat
   F438W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F438W.dat
+    path: filters/HST/WFC3/UVIS2/F438W.dat
   F475W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F475W.dat
+    path: filters/HST/WFC3/UVIS2/F475W.dat
   F555W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F555W.dat
+    path: filters/HST/WFC3/UVIS2/F555W.dat
   F625W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F625W.dat
+    path: filters/HST/WFC3/UVIS2/F625W.dat
   F814W:
     magsys: ab
     magzero: 0.0
-    path: HST/WFC3/UVIS2/F814W.dat
+    path: filters/HST/WFC3/UVIS2/F814W.dat
   H:
     magsys: vega
     magzero: 0.0
-    path: standard/2MASS_PAIRITEL/2MASS_PAIRITEL_H.dat
+    path: filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_H.dat
   H_AND:
     magsys: vega
     magzero: 0.0
-    path: CTIO/ANDICAM/Handicam.dat
+    path: filters/CTIO/ANDICAM/Handicam.dat
   H_P:
     magsys: vega
     magzero: 0.0
-    path: standard/Persson/hfilter
+    path: filters/standard/Persson/hfilter
   H_RC:
     magsys: vega
     magzero: 0.0
-    path: LCO/Swope/H_SWO_TAM_scan_atm.dat
+    path: filters/LCO/Swope/H_SWO_TAM_scan_atm.dat
   H_RCDP:
     magsys: vega
     magzero: 0.0
-    path: LCO/Dupont/H_RetroCam_duPont_TAMU_atm.dat
+    path: filters/LCO/Dupont/H_RetroCam_duPont_TAMU_atm.dat
   H_WIRC:
     magsys: vega
     magzero: 0.0
-    path: LCO/Dupont/H_DUP_TAM_scan_atm.dat
+    path: filters/LCO/Dupont/H_DUP_TAM_scan_atm.dat
   I:
     magsys: vega
     magzero: 0.0
-    path: standard/stritzinger/i_stritzinger
+    path: filters/standard/stritzinger/i_stritzinger
   J:
     magsys: vega
     magzero: 0.0
-    path: standard/2MASS_PAIRITEL/2MASS_PAIRITEL_J.dat
+    path: filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_J.dat
   J_AND:
     magsys: vega
     magzero: 0.0
-    path: CTIO/ANDICAM/Jandicam.dat
+    path: filters/CTIO/ANDICAM/Jandicam.dat
   J_P:
     magsys: vega
     magzero: 0.0
-    path: standard/Persson/jfilter
+    path: filters/standard/Persson/jfilter
   J_RC1:
     magsys: vega
     magzero: 0.0
-    path: LCO/Swope/Jrc1_SWO_TAM_scan_atm.dat
+    path: filters/LCO/Swope/Jrc1_SWO_TAM_scan_atm.dat
   J_RC2:
     magsys: vega
     magzero: 0.0
-    path: LCO/Swope/Jrc2_SWO_TAM_scan_atm.dat
+    path: filters/LCO/Swope/Jrc2_SWO_TAM_scan_atm.dat
   J_RCDP:
     magsys: vega
     magzero: 0.0
-    path: LCO/Dupont/J_RetroCam_duPont_TAMU_atm.dat
+    path: filters/LCO/Dupont/J_RetroCam_duPont_TAMU_atm.dat
   J_WIRC:
     magsys: vega
     magzero: 0.0
-    path: LCO/Dupont/J_DUP_TAM_scan_atm.dat
+    path: filters/LCO/Dupont/J_DUP_TAM_scan_atm.dat
   K:
     magsys: vega
     magzero: 0.0
-    path: standard/2MASS_PAIRITEL/2MASS_PAIRITEL_Ks.dat
+    path: filters/standard/2MASS_PAIRITEL/2MASS_PAIRITEL_Ks.dat
   K_AND:
     magsys: vega
     magzero: 0.0
-    path: CTIO/ANDICAM/Kandicam.dat
+    path: filters/CTIO/ANDICAM/Kandicam.dat
   K_P:
     magsys: vega
     magzero: 0.0
-    path: standard/Persson/kfilter
+    path: filters/standard/Persson/kfilter
   K_WIRC:
     magsys: vega
     magzero: 0.0
-    path: LCO/Dupont/K_DUP_TAM_scan_atm.dat
+    path: filters/LCO/Dupont/K_DUP_TAM_scan_atm.dat
   R:
     magsys: vega
     magzero: 0.0
-    path: standard/stritzinger/r_stritzinger
+    path: filters/standard/stritzinger/r_stritzinger
   U:
     magsys: vega
     magzero: 0.0
-    path: standard/stritzinger/u_stritzinger
+    path: filters/standard/stritzinger/u_stritzinger
   UVM2:
     magsys: vega
     magzero: 0.0
-    path: Swift/UVOT/photonUVM2.dat
+    path: filters/Swift/UVOT/photonUVM2.dat
   UVW1:
     magsys: vega
     magzero: 0.0
-    path: Swift/UVOT/photonUVW1.dat
+    path: filters/Swift/UVOT/photonUVW1.dat
   UVW2:
     magsys: vega
     magzero: 0.0
-    path: Swift/UVOT/photonUVW2.dat
+    path: filters/Swift/UVOT/photonUVW2.dat
   U_SWIFT:
     magsys: vega
     magzero: 0.0
-    path: Swift/UVOT/photonU_UVOT.dat
+    path: filters/Swift/UVOT/photonU_UVOT.dat
   V:
     magsys: vega
     magzero: 0.0
-    path: standard/stritzinger/v_stritzinger
+    path: filters/standard/stritzinger/v_stritzinger
   V_CSP:
     magsys: bd17
     magzero: 9.494
-    path: LCO/Swope/V_LC9844_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/V_LC9844_tel_ccd_atm_ext_1.2.dat
   V_CSP2:
     magsys: vega
     magzero: 0.03
-    path: LCO/Swope/V_CSP2_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/V_CSP2_tel_ccd_atm_ext_1.2.dat
   V_CSP_3009:
     magsys: bd17
     magzero: 9.488
-    path: LCO/Swope/V_LC3009_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/V_LC3009_tel_ccd_atm_ext_1.2.dat
   V_CSP_3014:
     magsys: bd17
     magzero: 9.492
-    path: LCO/Swope/V_LC3014_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/V_LC3014_tel_ccd_atm_ext_1.2.dat
   V_SWIFT:
     magsys: vega
     magzero: 0.0
-    path: Swift/UVOT/photonV_UVOT.dat
+    path: filters/Swift/UVOT/photonV_UVOT.dat
   Y_AND:
     magsys: vega
     magzero: 0.0
-    path: CTIO/ANDICAM/Yandicam.dat
+    path: filters/CTIO/ANDICAM/Yandicam.dat
   Y_P:
     magsys: vega
     magzero: 0.0
-    path: standard/Persson/yfilter
+    path: filters/standard/Persson/yfilter
   Y_RC:
     magsys: vega
     magzero: 0.0
-    path: LCO/Swope/Y_SWO_TAM_scan_atm.dat
+    path: filters/LCO/Swope/Y_SWO_TAM_scan_atm.dat
   Y_RCDP:
     magsys: vega
     magzero: 0.0
-    path: LCO/Dupont/Y_RetroCam_duPont_TAMU_atm.dat
+    path: filters/LCO/Dupont/Y_RetroCam_duPont_TAMU_atm.dat
   Y_WIRC:
     magsys: vega
     magzero: 0.0
-    path: LCO/Dupont/Y_DUP_TAM_scan_atm.dat
+    path: filters/LCO/Dupont/Y_DUP_TAM_scan_atm.dat
   g_CSP:
     magsys: bd17
     magzero: 9.644
-    path: LCO/Swope/g_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/g_tel_ccd_atm_ext_1.2.dat
   g_CSP2:
     magsys: bd17
     magzero: 9.64
-    path: LCO/Swope/g_CSP2_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/g_CSP2_tel_ccd_atm_ext_1.2.dat
   g_DES:
     magsys: ab
     magzero: 0.0
-    path: DECam/decam_g.txt
+    path: filters/DECam/decam_g.txt
   g_LSST:
     magsys: ab
     magzero: 0.0
-    path: LSST/2017-04_approx/LSST_g.dat
+    path: filters/LSST/2017-04_approx/LSST_g.dat
   g_PS1:
     magsys: ab
     magzero: 0.0
-    path: PS1/g_filt_revised.txt
+    path: filters/PS1/g_filt_revised.txt
   g_prime:
     magsys: bd17
     magzero: 9.64
-    path: USNO/USNO40/usno_g.res
+    path: filters/USNO/USNO40/usno_g.res
   i_CSP:
     magsys: bd17
     magzero: 9.25
-    path: LCO/Swope/i_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/i_tel_ccd_atm_ext_1.2.dat
   i_CSP2:
     magsys: bd17
     magzero: 9.25
-    path: LCO/Swope/i_CSP2_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/i_CSP2_tel_ccd_atm_ext_1.2.dat
   i_DES:
     magsys: ab
     magzero: 0.0
-    path: DECam/decam_i.txt
+    path: filters/DECam/decam_i.txt
   i_LSST:
     magsys: ab
     magzero: 0.0
-    path: LSST/2017-04_approx/LSST_i.dat
+    path: filters/LSST/2017-04_approx/LSST_i.dat
   i_PS1:
     magsys: ab
     magzero: 0.0
-    path: PS1/i_filt_tonry.txt
+    path: filters/PS1/i_filt_tonry.txt
   i_prime:
     magsys: bd17
     magzero: 9.25
-    path: USNO/USNO40/usno_i.res
+    path: filters/USNO/USNO40/usno_i.res
   p48g:
     magsys: ab
     magzero: 0.0
-    path: ZTF/p48g.txt
+    path: filters/ZTF/p48g.txt
   p48i:
     magsys: ab
     magzero: 0.0
-    path: ZTF/p48i.txt
+    path: filters/ZTF/p48i.txt
   p48r:
     magsys: ab
     magzero: 0.0
-    path: ZTF/p48r.txt
+    path: filters/ZTF/p48r.txt
   r_CSP:
     magsys: bd17
     magzero: 9.352
-    path: LCO/Swope/r_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/r_tel_ccd_atm_ext_1.2.dat
   r_CSP2:
     magsys: bd17
     magzero: 9.35
-    path: LCO/Swope/r_CSP2_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/r_CSP2_tel_ccd_atm_ext_1.2.dat
   r_DES:
     magsys: ab
     magzero: 0.0
-    path: DECam/decam_r.txt
+    path: filters/DECam/decam_r.txt
   r_LSST:
     magsys: ab
     magzero: 0.0
-    path: LSST/2017-04_approx/LSST_r.dat
+    path: filters/LSST/2017-04_approx/LSST_r.dat
   r_PS1:
     magsys: ab
     magzero: 0.0
-    path: PS1/r_filt_tonry.txt
+    path: filters/PS1/r_filt_tonry.txt
   r_prime:
     magsys: bd17
     magzero: 9.35
-    path: USNO/USNO40/usno_r.res
+    path: filters/USNO/USNO40/usno_r.res
   u_CSP:
     magsys: bd17
     magzero: 10.518
-    path: LCO/Swope/u_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/u_tel_ccd_atm_ext_1.2.dat
   u_CSP2:
     magsys: bd17
     magzero: 10.56
-    path: LCO/Swope/u_CSP2_tel_ccd_atm_ext_1.2.dat
+    path: filters/LCO/Swope/u_CSP2_tel_ccd_atm_ext_1.2.dat
   u_DES:
     magsys: ab
     magzero: 0.0
-    path: DECam/decam_u.txt
+    path: filters/DECam/decam_u.txt
   u_LSST:
     magsys: ab
     magzero: 0.0
-    path: LSST/2017-04_approx/LSST_u.dat
+    path: filters/LSST/2017-04_approx/LSST_u.dat
   u_prime:
     magsys: bd17
     magzero: 10.56
-    path: USNO/USNO40/usno_u.res
+    path: filters/USNO/USNO40/usno_u.res
   y_DES:
     magsys: ab
     magzero: 0.0
-    path: DECam/decam_y.txt
+    path: filters/DECam/decam_y.txt
   y_LSST:
     magsys: ab
     magzero: 0.0
-    path: LSST/2017-04_approx/LSST_y.dat
+    path: filters/LSST/2017-04_approx/LSST_y.dat
   y_PS1:
     magsys: ab
     magzero: 0.0
-    path: PS1/y_filt_tonry.txt
+    path: filters/PS1/y_filt_tonry.txt
   z_DES:
     magsys: ab
     magzero: 0.0
-    path: DECam/decam_z.txt
+    path: filters/DECam/decam_z.txt
   z_LSST:
     magsys: ab
     magzero: 0.0
-    path: LSST/2017-04_approx/LSST_z.dat
+    path: filters/LSST/2017-04_approx/LSST_z.dat
   z_PS1:
     magsys: ab
     magzero: 0.0
-    path: PS1/z_filt_tonry.txt
+    path: filters/PS1/z_filt_tonry.txt
   z_prime:
     magsys: bd17
     magzero: 9.23
-    path: USNO/USNO40/usno_z.res
+    path: filters/USNO/USNO40/usno_z.res
```

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/standards/alpha_lyr_stis_010.fits` & `bayesn-0.4.0/bayesn/bayesn-filters/standards/alpha_lyr_stis_010.fits`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn-filters/standards/bd_17d4708_stisnic_007.dat` & `bayesn-0.4.0/bayesn/bayesn-filters/standards/bd_17d4708_stisnic_007.dat`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn_io.py` & `bayesn-0.4.0/bayesn/bayesn_io.py`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/bayesn_model.py` & `bayesn-0.4.0/bayesn/bayesn_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from scipy.interpolate import interp1d
 from scipy.integrate import simpson
 import numpyro
 from numpyro.infer import MCMC, NUTS, init_to_median, init_to_sample, init_to_value, Predictive
 import numpyro.distributions as dist
 from numpyro.optim import Adam
 from numpyro.infer import SVI, Trace_ELBO
-from numpyro.infer.autoguide import AutoDelta
+from numpyro.infer.autoguide import AutoDelta, AutoMultivariateNormal, AutoDiagonalNormal, AutoLaplaceApproximation
 import h5py
 import sncosmo
 from .spline_utils import invKD_irr, spline_coeffs_irr
 from .bayesn_io import write_snana_lcfile
 import pickle
 import pandas as pd
 import jax
@@ -39,14 +39,15 @@
 import extinction
 import timeit
 from astropy.io import fits
 from ruamel.yaml import YAML
 import time
 from tqdm import tqdm
 from astropy.table import QTable
+from .zltn_utils import *
 
 yaml = YAML(typ='safe')
 yaml.default_flow_style = False
 
 jax.config.update('jax_enable_x64', True)  # Enables 64 computation
 
 np.seterr(divide='ignore', invalid='ignore')  # Disable divide by zero warnings
@@ -202,18 +203,15 @@
         self.end_time = None
         # os.environ['XLA_PYTHON_CLIENT_PREALLOCATE'] = 'false'
         print('Current devices:', jax.devices())
 
         self.__root_dir__ = os.path.dirname(os.path.abspath(__file__))
         print(f'Currently working in {os.getcwd()}')
 
-        # Use built-in filters if filters.yaml is not provided
-        if filter_yaml is None:
-            filter_yaml = os.path.join(self.__root_dir__, 'bayesn-filters', 'filters.yaml')
-
+        # Load built-in filter_yaml and add custom filters if specified
         self.cosmo = FlatLambdaCDM(**fiducial_cosmology)
         self.data = None
         self.hsiao_interp = None
         self.RV_MW = device_put(jnp.array(3.1))
         self.sigma_pec = device_put(jnp.array(150 / 3e5))
         self.sn_list = None
         self.filter_yaml = filter_yaml
@@ -227,14 +225,17 @@
             print(f'Loading built-in model {load_model}')
             with open(os.path.join(self.__root_dir__, 'model_files', load_model, 'BAYESN.YAML'), 'r') as file:
                 params = yaml.load(file)
         else:
             raise FileNotFoundError(f'Specified model {load_model} does not exist and does not correspond to one '
                                     f'of the built-in model {built_in_models}')
 
+        # Define example light curve for jupyter notebook demos
+        self.example_lc = os.path.join(self.__root_dir__, 'data', 'example_lcs', 'Foundation_DR1_2016W.txt')
+
         self.l_knots = jnp.array(params['L_KNOTS'])
         self.tau_knots = jnp.array(params['TAU_KNOTS'])
         self.W0 = jnp.array(params['W0'])
         self.W1 = jnp.array(params['W1'])
         self.L_Sigma = jnp.array(params['L_SIGMA_EPSILON'])
         self.M0 = jnp.array(params['M0'])
         self.sigma0 = jnp.array(params['SIGMA0'])
@@ -323,60 +324,91 @@
         # Oversampling must be odd.
         assert self.band_oversampling % 2 == 1
         pad = (self.band_oversampling - 1) // 2
         band_log_wave = np.arange(np.log10(self.min_wave),
                                   band_max_log_wave, band_spacing)
         band_wave = 10 ** band_log_wave
 
-        if not os.path.exists(self.filter_yaml):
-            raise FileNotFoundError(f'Specified filter yaml {self.filter_yaml} does not exist')
-        with open(self.filter_yaml, 'r') as file:
+        # Load in-built filter yaml first
+        with open(os.path.join(self.__root_dir__, 'bayesn-filters', 'filters.yaml'), 'r') as file:
             filter_dict = yaml.load(file)
 
-        # Load standard spectra if necessary, AB is just calculated analytically so no standard spectrum is required----
-        if 'standards' in filter_dict.keys():
-            if 'standards_root' in filter_dict.keys():
-                standards_root = filter_dict['standards_root']
+        # Prepend root locations for in-built filters
+        for key, val in filter_dict['standards'].items():
+            filter_dict['standards'][key]['path'] = os.path.join(self.__root_dir__, 'bayesn-filters', val['path'])
+
+        for key, val in filter_dict['filters'].items():
+            filter_dict['filters'][key]['path'] = os.path.join(self.__root_dir__, 'bayesn-filters', val['path'])
+
+        # Add custom filters, if specified
+        if self.filter_yaml is not None:
+            if not os.path.exists(self.filter_yaml):
+                raise FileNotFoundError(f'Specified filter yaml {self.filter_yaml} does not exist')
+            with open(self.filter_yaml, 'r') as file:
+                custom_filter_dict = yaml.load(file)
+            # Add custom standards if specified---------------------
+            if 'standards' in custom_filter_dict.keys():
+                if 'standards_root' in custom_filter_dict.keys():
+                    standards_root = custom_filter_dict['standards_root']
+                else:
+                    standards_root = ''
+                for key, val in custom_filter_dict['standards'].items():
+                    path = os.path.join(standards_root, val['path'])
+                    # Fill environment variables if used e.g. $SNDATA_ROOT
+                    split_path = os.path.normpath(path).split(os.path.sep)
+                    root = split_path[0]
+                    if root[:1] == '$':
+                        env = os.getenv(root[1:])
+                        if env is None:
+                            raise FileNotFoundError(f'The environment variable {root} was not found')
+                        path = os.path.join(env, *split_path[1:])
+                    elif not os.path.isabs(path):  # If relative path, prepend yaml location
+                        path = os.path.join(os.path.split(os.path.abspath(self.filter_yaml))[0], path)
+                    custom_filter_dict['standards'][key]['path'] = path
+                    # Add custom standard and overwrite existing one of same name if present
+                    filter_dict['standards'][key] = custom_filter_dict['standards'][key]
+            # Add custom filters
+            if 'filters_root' in custom_filter_dict.keys():
+                filters_root = custom_filter_dict['filters_root']
             else:
-                standards_root = ''
-            for key, val in filter_dict['standards'].items():
-                path = os.path.join(standards_root, val['path'])
+                filters_root = ''
+            for key, val in custom_filter_dict['filters'].items():
+                path = os.path.join(filters_root, val['path'])
                 # Fill environment variables if used e.g. $SNDATA_ROOT
                 split_path = os.path.normpath(path).split(os.path.sep)
                 root = split_path[0]
                 if root[:1] == '$':
                     env = os.getenv(root[1:])
                     if env is None:
                         raise FileNotFoundError(f'The environment variable {root} was not found')
                     path = os.path.join(env, *split_path[1:])
                 elif not os.path.isabs(path):  # If relative path, prepend yaml location
-                    path = os.path.join(os.path.split(self.filter_yaml)[0], path)
-                if '.fits' in path:  # If fits file
-                    with fits.open(path) as hdu:
-                        standard_df = pd.DataFrame.from_records(hdu[1].data)
-                    standard_lam, standard_f = standard_df.WAVELENGTH.values, standard_df.FLUX.values
-                else:
-                    standard_txt = np.loadtxt(path)
-                    standard_lam, standard_f = standard_txt[:, 0], standard_txt[:, 1]
-                filter_dict['standards'][key]['lam'] = standard_lam
-                filter_dict['standards'][key]['f_lam'] = standard_f
-        else:
-            print('You have not provided any standard spectra e.g. Vega in filter input yaml, this is fine as long '
-                  'as everything is AB, otherwise make sure to add this')
+                    path = os.path.join(os.path.split(os.path.abspath(self.filter_yaml))[0], path)
+                custom_filter_dict['filters'][key]['path'] = path
+                # Add custom filter and overwrite existing one of same name if present
+                filter_dict['filters'][key] = custom_filter_dict['filters'][key]
+
+        # Load standard spectra if necessary, AB is just calculated analytically so no standard spectrum is required----
+        for key, val in filter_dict['standards'].items():
+            path = val['path']
+            if '.fits' in path:  # If fits file
+                with fits.open(path) as hdu:
+                    standard_df = pd.DataFrame.from_records(hdu[1].data)
+                standard_lam, standard_f = standard_df.WAVELENGTH.values, standard_df.FLUX.values
+            else:
+                standard_txt = np.loadtxt(path)
+                standard_lam, standard_f = standard_txt[:, 0], standard_txt[:, 1]
+            filter_dict['standards'][key]['lam'] = standard_lam
+            filter_dict['standards'][key]['f_lam'] = standard_f
 
         def ab_standard_flam(l):  # Can just use analytic function for AB spectrum
             f = (const.c.to('AA/s').value / 1e23) * (l ** -2) * 10 ** (-48.6 / 2.5) * 1e23
             return f
 
         # Load filters------------------------------
-        if 'filters_root' in filter_dict.keys():
-            filters_root = filter_dict['filters_root']
-        else:
-            filters_root = ''
-
         band_weights, zps, offsets = [], [], []
         self.band_dict, self.zp_dict, self.band_lim_dict = {}, {}, {}
 
         # Prepare NULL band. This is a fake band with a very wide wavelength range used only for padded data points to
         # ensure that these padded data points never fall out of the wavelength coverage of the model. These padded
         # data points do not contribute to the likelihood in any way, this is entirely for computational reasons
         self.band_dict['NULL_BAND'] = 0
@@ -384,30 +416,19 @@
         self.band_lim_dict['NULL_BAND'] = band_wave[0], band_wave[-1]
         band_weights.append(np.ones_like(band_wave))
         zps.append(10)
         offsets.append(0)
 
         band_ind = 1
         for key, val in filter_dict['filters'].items():
-            path = os.path.join(filters_root, val['path'])
-            # Fill environment variables if used e.g. $SNDATA_ROOT
-            split_path = os.path.normpath(path).split(os.path.sep)
-            root = split_path[0]
-            if root[:1] == '$':
-                env = os.getenv(root[1:])
-                if env is None:
-                    raise FileNotFoundError(f'The environment variable {root} was not found')
-                path = os.path.join(env, *split_path[1:])
-            elif not os.path.isabs(path):  # If relative path, prepend yaml location
-                path = os.path.join(os.path.split(self.filter_yaml)[0], path)
             band, magsys, offset = key, val['magsys'], val['magzero']
             try:
-                R = np.loadtxt(path)
+                R = np.loadtxt(val['path'])
             except:
-                raise FileNotFoundError(f'Filter response not found for {key}')
+                raise FileNotFoundError(f'Filter response file {val["path"]} not found for {key}')
 
             # Convert wavelength units if required, model is defined in Angstroms
             units = val.get('lam_unit', 'AA')
             if units.lower() == 'nm':  # Convert from nanometres to Angstroms
                 R[:, 0] = R[:, 0] * 10
             elif units.lower() == 'micron':  # Convert from microns to Angstroms
                 R[:, 0] = R[:, 0] * 1e4
@@ -767,34 +788,50 @@
 
         X = X.at[q].set(X[q] + a * interp)
         X = X.at[q + 1].set(X[q + 1] + b * interp)
         X = X.at[:].set(X[:] + c * invkd[q, :] * interp + d * invkd[q + 1, :] * interp)
 
         return X
 
-    def fit_model_globalRV(self, obs, weights):
+    def fit_model_globalRV(self, obs, weights, fix_tmax=False, fix_theta=False, theta_val=0, fix_AV=False, AV_val=0):
         """
         Numpyro model used for fitting latent SN properties with single global RV. Will fit for time of maximum as well
         as theta, epsilon, AV and distance modulus.
 
         Parameters
         ----------
         obs: array-like
             Data to fit, from output of process_dataset
         weights: array-like
             Band-weights to calculate photometry
+        fix_tmax: Boolean, optional
+            If True, tmax will be fixed to fiducial value and will not be inferred. Defaults to False
+        fix_theta: Boolean, optional
+            If True, theta will be fixed to value specified by theta_val. Defaults to False.
+        theta_val: float or array-like, optional
+            Value to fix theta to, if fix_theta=True. Defaults to 0
+        fix_AV: Boolean, optional
+            If True, AV will be fixed to value specified by theta_AV. Defaults to False.
+        AV_val: float or array-like, optional
+            Value to fix AV to, if fix_AV=True. Defaults to 0
+
+        Returns
+        -------
 
         """
         sample_size = obs.shape[-1]
         N_knots_sig = (self.l_knots.shape[0] - 2) * self.tau_knots.shape[0]
 
         with numpyro.plate('SNe', sample_size) as sn_index:
             theta = numpyro.sample(f'theta', dist.Normal(0, 1.0))
+            theta = theta * (1 - fix_theta) + theta_val * fix_theta
             AV = numpyro.sample(f'AV', dist.Exponential(1 / self.tauA))
+            AV = AV * (1 - fix_AV) + AV_val * fix_AV
             tmax = numpyro.sample('tmax', dist.Uniform(-10, 10))
+            tmax = tmax * (1 - fix_tmax)
             t = obs[0, ...] - tmax[None, sn_index]
             hsiao_interp = jnp.array([19 + jnp.floor(t), 19 + jnp.ceil(t), jnp.remainder(t, 1)])
             keep_shape = t.shape
             t = t.flatten(order='F')
             J_t = self.J_t_map(t, self.tau_knots, self.KD_t).reshape((*keep_shape, self.tau_knots.shape[0]),
                                                                      order='F').transpose(1, 2, 0)
             eps_mu = jnp.zeros(N_knots_sig)
@@ -815,39 +852,101 @@
             Ds = numpyro.sample('Ds', dist.Normal(muhat, Ds_err))  # Ds_err
             flux = self.get_flux_batch(self.M0, theta, AV, self.W0, self.W1, eps, Ds, self.RV, band_indices, mask,
                                        J_t, hsiao_interp, weights)
             with numpyro.handlers.mask(mask=mask):
                 numpyro.sample(f'obs', dist.Normal(flux, obs[2, :, sn_index].T),
                                obs=obs[1, :, sn_index].T)
 
-    def fit_model_popRV(self, obs, weights):
+    def fit_model_globalRV_vi(self, obs, weights):
+        """
+        Numpyro model used for fitting SN properties assuming fixed global properties from a trained model. Will fit for
+        tmax as well as theta, epsilon, Av and distance modulus. This model is slightly modified for ZLTN VI.
+
+        Parameters
+        ----------
+        obs: array-like
+            Data to fit, from output of process_dataset
+        weights: array-like
+            Band-weights to calculate photometry
+
+        """
+        sample_size = obs.shape[-1]
+        N_knots_sig = (self.l_knots.shape[0] - 2) * self.tau_knots.shape[0]
+
+        with numpyro.plate('SNe', sample_size) as sn_index:
+            AV = numpyro.sample(f'AV', My_Exponential(1 / self.tauA))
+            theta = numpyro.sample(f'theta', dist.Normal(0, 1.0))
+            tmax = numpyro.sample('tmax', dist.Uniform(-10, 10))
+
+            t = obs[0, ...] - tmax[None, sn_index]
+            hsiao_interp = jnp.array([19 + jnp.floor(t), 19 + jnp.ceil(t), jnp.remainder(t, 1)])
+            keep_shape = t.shape
+            t = t.flatten(order='F')
+            J_t = self.J_t_map(t, self.tau_knots, self.KD_t).reshape((*keep_shape, self.tau_knots.shape[0]),
+                                                                     order='F').transpose(1, 2, 0)
+            eps_mu = jnp.zeros(N_knots_sig)
+            eps_tform = numpyro.sample('eps_tform', dist.MultivariateNormal(eps_mu, jnp.eye(N_knots_sig)))
+            eps_tform = eps_tform.T
+            eps = numpyro.deterministic('eps', jnp.matmul(self.L_Sigma, eps_tform))
+            eps = eps.T
+            eps = jnp.reshape(eps, (sample_size, self.l_knots.shape[0] - 2, self.tau_knots.shape[0]), order='F')
+            eps_full = jnp.zeros((sample_size, self.l_knots.shape[0], self.tau_knots.shape[0]))
+            eps = eps_full.at[:, 1:-1, :].set(eps)
+            # eps = jnp.zeros((sample_size, self.l_knots.shape[0], self.tau_knots.shape[0]))
+            band_indices = obs[-6, :, sn_index].astype(int).T
+            muhat = obs[-3, 0, sn_index]
+            mask = obs[-1, :, sn_index].T.astype(bool)
+            muhat_err = 5
+            Ds_err = jnp.sqrt(muhat_err * muhat_err + self.sigma0 * self.sigma0)
+
+            Ds = numpyro.sample('Ds', dist.Normal(muhat, Ds_err))  # Ds_err
+            flux = self.get_flux_batch(self.M0, theta, AV, self.W0, self.W1, eps, Ds, self.RV, band_indices, mask,
+                                       J_t, hsiao_interp, weights)
+            with numpyro.handlers.mask(mask=mask):
+                numpyro.sample(f'obs', dist.Normal(flux, obs[2, :, sn_index].T),
+                               obs=obs[1, :, sn_index].T)
+
+    def fit_model_popRV(self, obs, weights, fix_tmax=False, fix_theta=False, theta_val=0, fix_AV=False, AV_val=0):
         """
         Numpyro model used for fitting latent SN properties with a truncated Gaussian prior on RV. Will fit for time of
         maximum as well as theta, epsilon, AV, RV and distance modulus.
 
         Parameters
         ----------
         obs: array-like
             Data to fit, from output of process_dataset
         weights: array-like
             Band-weights to calculate photometry
+        fix_tmax: Boolean, optional
+            If True, tmax will be fixed to fiducial value and will not be inferred. Defaults to False
+        fix_theta: Boolean, optional
+            If True, theta will be fixed to value specified by theta_val. Defaults to False.
+        theta_val: float or array-like, optional
+            Value to fix theta to, if fix_theta=True. Defaults to 0
+        fix_AV: Boolean, optional
+            If True, AV will be fixed to value specified by theta_AV. Defaults to False.
+        AV_val: float or array-like, optional
+            Value to fix AV to, if fix_AV=True. Defaults to 0
 
         """
         sample_size = obs.shape[-1]
         N_knots_sig = (self.l_knots.shape[0] - 2) * self.tau_knots.shape[0]
         phi_alpha_R = norm.cdf((self.trunc_val - self.mu_R) / self.sigma_R)
 
         with numpyro.plate('SNe', sample_size) as sn_index:
             theta = numpyro.sample(f'theta', dist.Normal(0, 1.0))
+            theta = theta * (1 - fix_theta) + theta_val * fix_theta
             AV = numpyro.sample(f'AV', dist.Exponential(1 / self.tauA))
+            AV = AV * (1 - fix_AV) + AV_val * fix_AV
+            tmax = numpyro.sample('tmax', dist.Uniform(-10, 10))
+            tmax = tmax * (1 - fix_tmax)
             RV_tform = numpyro.sample('RV_tform', dist.Uniform(0, 1))
-            RV = numpyro.deterministic('Rv_LM',
+            RV = numpyro.deterministic('Rv',
                                        self.mu_R + self.sigma_R * ndtri(phi_alpha_R + RV_tform * (1 - phi_alpha_R)))
 
-            tmax = numpyro.sample('tmax', dist.Uniform(-10, 10))
             t = obs[0, ...] - tmax[None, sn_index]
             hsiao_interp = jnp.array([19 + jnp.floor(t), 19 + jnp.ceil(t), jnp.remainder(t, 1)])
             keep_shape = t.shape
             t = t.flatten(order='F')
             J_t = self.J_t_map(t, self.tau_knots, self.KD_t).reshape((*keep_shape, self.tau_knots.shape[0]),
                                                                      order='F').transpose(1, 2, 0)
             eps_mu = jnp.zeros(N_knots_sig)
@@ -868,14 +967,67 @@
             Ds = numpyro.sample('Ds', dist.Normal(muhat, Ds_err))  # Ds_err
             flux = self.get_flux_batch(self.M0, theta, AV, self.W0, self.W1, eps, Ds, RV, band_indices, mask,
                                        J_t, hsiao_interp, weights)
             with numpyro.handlers.mask(mask=mask):
                 numpyro.sample(f'obs', dist.Normal(flux, obs[2, :, sn_index].T),
                                obs=obs[1, :, sn_index].T)  # _{sn_index}
 
+    def fit_model_popRV_vi(self, obs, weights):
+        """
+        Numpyro model used for fitting latent SN properties with a truncated Gaussian prior on RV. Will fit for time of
+        maximum as well as theta, epsilon, AV, RV and distance modulus. This model is slightly modified for ZLTN VI.
+
+        Parameters
+        ----------
+        obs: array-like
+            Data to fit, from output of process_dataset
+        weights: array-like
+            Band-weights to calculate photometry
+
+        """
+        sample_size = obs.shape[-1]
+        N_knots_sig = (self.l_knots.shape[0] - 2) * self.tau_knots.shape[0]
+        phi_alpha_R = norm.cdf((self.trunc_val - self.mu_R) / self.sigma_R)
+
+        with numpyro.plate('SNe', sample_size) as sn_index:
+            AV = numpyro.sample(f'AV', My_Exponential(1 / self.tauA))
+            RV_tform = numpyro.sample('RV_tform', dist.Uniform(0, 1))
+            RV = numpyro.deterministic('Rv',
+                                       self.mu_R + self.sigma_R * ndtri(phi_alpha_R + RV_tform * (1 - phi_alpha_R)))
+            theta = numpyro.sample(f'theta', dist.Normal(0, 1.0))
+            tmax = numpyro.sample('tmax', dist.Uniform(-10, 10))
+
+            t = obs[0, ...] - tmax[None, sn_index]
+            hsiao_interp = jnp.array([19 + jnp.floor(t), 19 + jnp.ceil(t), jnp.remainder(t, 1)])
+            keep_shape = t.shape
+            t = t.flatten(order='F')
+            J_t = self.J_t_map(t, self.tau_knots, self.KD_t).reshape((*keep_shape, self.tau_knots.shape[0]),
+                                                                     order='F').transpose(1, 2, 0)
+            eps_mu = jnp.zeros(N_knots_sig)
+            eps_tform = numpyro.sample('eps_tform', dist.MultivariateNormal(eps_mu, jnp.eye(N_knots_sig)))
+            eps_tform = eps_tform.T
+            eps = numpyro.deterministic('eps', jnp.matmul(self.L_Sigma, eps_tform))
+            eps = eps.T
+            eps = jnp.reshape(eps, (sample_size, self.l_knots.shape[0] - 2, self.tau_knots.shape[0]), order='F')
+            eps_full = jnp.zeros((sample_size, self.l_knots.shape[0], self.tau_knots.shape[0]))
+            eps = eps_full.at[:, 1:-1, :].set(eps)
+            # eps = jnp.zeros((sample_size, self.l_knots.shape[0], self.tau_knots.shape[0]))
+            band_indices = obs[-6, :, sn_index].astype(int).T
+            muhat = obs[-3, 0, sn_index]
+            mask = obs[-1, :, sn_index].T.astype(bool)
+            muhat_err = 5
+            Ds_err = jnp.sqrt(muhat_err * muhat_err + self.sigma0 * self.sigma0)
+
+            Ds = numpyro.sample('Ds', dist.Normal(muhat, Ds_err))  # Ds_err
+            flux = self.get_flux_batch(self.M0, theta, AV, self.W0, self.W1, eps, Ds, RV, band_indices, mask,
+                                       J_t, hsiao_interp, weights)
+            with numpyro.handlers.mask(mask=mask):
+                numpyro.sample(f'obs', dist.Normal(flux, obs[2, :, sn_index].T),
+                               obs=obs[1, :, sn_index].T)
+
     def train_model_globalRV(self, obs, weights):
         """
         Numpyro model used for training to learn global parameters, assuming a single global RV
 
         Parameters
         ----------
         obs: array-like
@@ -1440,14 +1592,15 @@
         args.pop('CONFIG', None)
         args.pop('config', None)
 
         # Set default parameters for some parameters if not specified in input.yaml or command line
         args['num_chains'] = args.get('num_chains', 4)
         args['num_warmup'] = args.get('num_warmup', 500)
         args['num_samples'] = args.get('num_samples', 500)
+        args['fit_method'] = args.get('fit_method', 'mcmc')
         args['chain_method'] = args.get('chain_method', 'parallel')
         args['initialisation'] = args.get('initialisation', 'median')
         args['l_knots'] = args.get('l_knots', self.l_knots.tolist())
         args['tau_knots'] = args.get('tau_knots', self.tau_knots.tolist())
         args['map'] = args.get('map', {})
         args['drop_bands'] = args.get('drop_bands', [])
         args['outputdir'] = args.get('outputdir', os.path.join(os.getcwd()))
@@ -1469,14 +1622,19 @@
         if not (args['mode'] == 'fitting' and args['snana']):
             try:
                 if not os.path.exists(args['outputdir']):
                     os.mkdir(args['outputdir'])
             except FileNotFoundError:
                 raise FileNotFoundError('Requested output directory does not exist and could not be created')
 
+        # Check fit method is valid
+        args['fit_method'] = args['fit_method'].lower()
+        if args['fit_method'].lower() not in ['vi', 'mcmc']:
+            raise ValueError(f'Requested fitting method {args["fit_method"]}, must be one of "mcmc" or "vi"')
+
         if 'training' in args['mode'].lower():
             self.l_knots = device_put(np.array(args['l_knots'], dtype=float))
             self._setup_band_weights()
             KD_l = invKD_irr(self.l_knots)
             self.J_l_T = device_put(spline_coeffs_irr(self.model_wave, self.l_knots, KD_l))
             self.tau_knots = device_put(np.array(args['tau_knots'], dtype=float))
             self.KD_t = device_put(invKD_irr(self.tau_knots))
@@ -1510,14 +1668,15 @@
             init_strategy = init_to_median()
         elif args['initialisation'] == 'sample':
             init_strategy = init_to_sample()
         else:
             init_strategy = init_to_value(values=self.initial_guess(args, reference_model=args['initialisation']))
 
         print(f'Current mode: {args["mode"]}')
+        print('Running...')
 
         if args['mode'].lower() == 'training_globalrv':
             nuts_kernel = NUTS(self.train_model_globalRV, adapt_step_size=True, target_accept_prob=0.8,
                                init_strategy=init_strategy,
                                dense_mass=False, find_heuristic_step_size=False, regularize_mass_matrix=False,
                                step_size=0.1)
         elif args['mode'].lower() == 'training_poprv':
@@ -1552,27 +1711,372 @@
             elif self.model_type == 'fixed_RV':
                 nuts_kernel = NUTS(self.fit_model_globalRV, adapt_step_size=True, init_strategy=init_strategy,
                                    max_tree_depth=10)
         else:
             raise ValueError("Invalid mode, must select one of 'training_globalRV', 'training_popRV', 'fitting',"
                              "'dust', 'dust_split_mag', 'dust_split_sed' or 'dust_redshift'")
 
-        mcmc = MCMC(nuts_kernel, num_samples=args['num_samples'], num_warmup=args['num_warmup'],
+        # self.data, self.band_weights = self.data[..., 1:2], self.band_weights[1:2, ...]
+
+        if args['mode'].lower() == 'fitting' and args['fit_method'] == 'mcmc':  # Use vmap to vectorise over individual fitting jobs
+            def fit_vmap_mcmc(data, weights):
+                """
+                Short function-in-a-function just to allow you to do a vectorised map over multiple objects on a single
+                device
+
+                Parameters
+                ----------
+                obs: array-like
+                    Data to fit, from output of process_dataset
+                weights: array-like
+                    Band-weights to calculate photometry
+
+                Returns
+                -------
+
+                sample_dict: dict
+                    Samples and other information from MCMC fit
+
+                """
+                rng_key = PRNGKey(0)
+                mcmc = MCMC(nuts_kernel, num_samples=args['num_samples'], num_warmup=args['num_warmup'],
+                            num_chains=args['num_chains'], chain_method=args['chain_method'], progress_bar=False)
+                mcmc.run(rng_key, data[..., None], weights[None, ...])
+                return {**mcmc.get_samples(group_by_chain=True), **mcmc.get_extra_fields(group_by_chain=True)}
+
+            start = timeit.default_timer()
+            map = jax.vmap(fit_vmap_mcmc, in_axes=(2, 0))
+            samples = map(self.data, self.band_weights)
+            expand_dim = False
+            for key, val in samples.items():
+                val = np.squeeze(val)
+                if len(val.shape) == 2:  # In case fitting only one object
+                    expand_dim = True
+                if expand_dim:
+                    val = val[None, ...]
+                if len(val.shape) == 4:
+                    samples[key] = val.transpose(1, 2, 0, 3)
+                else:
+                    samples[key] = val.transpose(1, 2, 0)
+            end = timeit.default_timer()
+        elif args['mode'].lower() == 'fitting' and args['fit_method'] == 'vi':
+            def fit_vmap_vi(data, weights):
+                """
+                Short function-in-a-function just to allow you to do a vectorised map over multiple objects on a single
+                device
+
+                Parameters
+                ----------
+                obs: array-like
+                    Data to fit, from output of process_dataset
+                weights: array-like
+                    Band-weights to calculate photometry
+
+                Returns
+                -------
+
+                sample_dict: dict
+                    Samples and other information from MCMC fit
+
+                """
+                optimizer = Adam(0.01)
+                model = self.fit_model_globalRV
+                sample_locs = ['AV', 'theta', 'tmax', 'eps_tform', 'Ds']
+                # First start with the Laplace Approximation
+                laplace_guide = AutoLaplaceApproximation(model, init_loc_fn=init_strategy)
+                svi = SVI(model, laplace_guide, optimizer, loss=Trace_ELBO(5))
+
+                svi_result = svi.run(PRNGKey(123), 15000, data[..., None], weights[None, ...], progress_bar=False)
+                params, losses = svi_result.params, svi_result.losses
+                laplace_median = laplace_guide.median(params)
+
+                # Now initialize the ZLTN guide on the Laplace Approximation median (just for AV, theta, and mu)
+                new_init_dict = {k: jnp.array([laplace_median[k][0]]) for k in sample_locs if k in laplace_median}
+                model = self.fit_model_globalRV_vi
+                zltn_guide = AutoMultiZLTNGuide(model, init_loc_fn=init_to_value(values=new_init_dict))
+
+                # svi_result = fit_zltn_vmap(model, zltn_guide, data[..., None], weights[None, ...])
+                svi = SVI(model, zltn_guide, Adam(0.005), Trace_ELBO(5))
+                svi_result = svi.run(PRNGKey(123), 10000, data[..., None], weights[None, ...], progress_bar=False)
+                params, losses = svi_result.params, svi_result.losses
+                predictive = Predictive(zltn_guide, params=params, num_samples=4 * args['num_samples'])
+                samples = predictive(PRNGKey(123), data=None)
+                # samples['losses'] = losses
+                return {**samples}
+
+            start = timeit.default_timer()
+            map = jax.vmap(fit_vmap_vi, in_axes=(2, 0))
+            samples = map(self.data, self.band_weights)
+            del samples['_auto_latent']
+            expand_dim = False
+            for key, val in samples.items():
+                val = np.squeeze(val)
+                if len(val.shape) == 1:  # In case fitting only one object
+                    expand_dim = True
+                if expand_dim:
+                    val = val[None, ...]
+                if len(val.shape) == 3:
+                    samples[key] = val.transpose(1, 2, 0)
+                else:
+                    samples[key] = val.transpose()
+                samples[key] = samples[key].reshape(4, args['num_samples'], *samples[key].shape[1:])
+            end = timeit.default_timer()
+        else:
+            mcmc = MCMC(nuts_kernel, num_samples=args['num_samples'], num_warmup=args['num_warmup'],
                     num_chains=args['num_chains'],
                     chain_method=args['chain_method'])
+            rng = PRNGKey(0)
+            start = timeit.default_timer()
+
+            mcmc.run(rng, self.data, self.band_weights, extra_fields=('potential_energy',))
+            end = timeit.default_timer()
+            mcmc.print_summary()
+            samples = mcmc.get_samples(group_by_chain=True)
+        print(f'Total inference runtime: {end - start} seconds')
+        self.postprocess(samples, args)
+
+    def fit_from_file(self, path, filt_map={}, peak_mjd_key='SEARCH_PEAKMJD', print_summary=True, file_prefix=None,
+                      drop_bands=[], fix_tmax=False, fix_theta=False, fix_AV=False, RV=False, mu_R=False, sigma_R=False,
+                      mag=False):
+        """
+        Method to fit light curve contained in SNANA-format text file using BayeSN model
+
+        Parameters
+        ----------
+        path: str
+            Path to SNANA-format text file containing data to be fit
+        filt_map: dict, optional
+            Dictionary providing mapping between filter names in file and BayeSN filters. Defaults to empty dictionary
+        peak_mjd_key: str, optional
+            Key to be used for peak MJD in SNANA text file meta. Defaults to 'SEARCH_PEAKMJD'
+        print_summary: Boolean, optional
+            Specifies whether to print fit summary
+        file_prefix: str, optional
+            Prefix of name for output files containing summary table and MCMC samples. Default to None, in which case
+            output files will not be saved and only returned for use in script.
+        drop_bands: array-like, optional
+            List of bands to be ignored during fitting. Defaults to empty list
+        fix_tmax: Boolean, optional
+            If True, tmax will not be inferred and fiducial value in file meta will be fixed. Defaults to False.
+        fix_theta: float, optional
+            Value to fix theta at during fitting. Defaults to False, meaning that theta will be inferred during fitting
+            rather than fixed.
+        fix_AV: float, optional
+            Value to fix AV at during fitting. Defaults to False, meaning that AV will be inferred during fitting
+            rather than fixed.
+        RV: float, optional
+            Value to fix RV at during fitting. Defaults to False, meaning that default model RV treatment will be used.
+        mu_R: float, optional
+            Value of mean of RV distribution to be used during fitting. Defaults to False, meaning that default model
+            RV treatment will be used. If specified, sigma_R must also be specified.
+        sigma_R: float, optional
+            Value of standard deviation of RV distribution. Defaults to False, meaning that default model RV treatment
+            will be used.
+        mag: Boolean, optional
+            Specifies whether data is mag or flux. If True, data is assumed to be mag and is automatically converted to
+            flux before fitting.
+
+        Returns
+        -------
+
+        samples: dict
+            Dictionary containing parameter names as keys and MCMC samples as values
+        sn_props: tuple
+            Tuple containing SN redshift and MW E(B-V), which can be useful to have in memory when making plots
+
+        """
+        meta, lcdata = sncosmo.read_snana_ascii(path, default_tablename='OBS')
+        lcdata = lcdata['OBS'].to_pandas()
+
+        t = lcdata.MJD.values
+        flux = lcdata.FLUXCAL.values
+        flux_err = lcdata.FLUXCALERR.values
+        filters = lcdata.FLT.values
+        peak_mjd = meta[peak_mjd_key]
+        z = meta['REDSHIFT_HELIO']
+        ebv_mw = meta['MWEBV']
+
+        samples, sn_props = self.fit(t, flux, flux_err, filters, z, ebv_mw=ebv_mw, peak_mjd=peak_mjd, filt_map=filt_map,
+                                     print_summary=print_summary, file_prefix=file_prefix, drop_bands=drop_bands,
+                                     fix_tmax=fix_tmax, fix_theta=fix_theta, fix_AV=fix_AV, RV=RV, mu_R=mu_R,
+                                     sigma_R=sigma_R, mag=mag)
+
+        return samples, sn_props
+
+    def fit(self, t, flux, flux_err, filters, z, ebv_mw=0, peak_mjd=None, filt_map={}, print_summary=True,
+            file_prefix=None, drop_bands=[], fix_tmax=False, fix_theta=False, fix_AV=False, RV=False, mu_R=False,
+            sigma_R=False, mag=False):
+        """
+        Method to fit light curve data loaded into memory with BayeSN model
+
+        Parameters
+        ----------
+        t: array-like
+            Set of MJDs/rest-frame phases for light curve data to be fit. If you pass MJD and also a peak_mjd, values
+            will automatically be converted to rest-frame phases
+        flux: array-like
+            Set of fluxes/mags for light curve data to be fit. Despite the name, you can use mags and if mag=True data
+            will be automatically converted into flux for fitting.
+        flux_err: array-like
+            Set of flux/mag errors for light curve data to be fit. Despite the name, you can use mags and if mag=True
+            data will be automatically converted into flux for fitting.
+        filters: array-like
+            Set of filters that flux/flux_err are measurements for, telling BayeSN which filters to use when fitting
+            data. Must be of same length as flux/flux_err i.e. specify the filter for each data point individually
+        z: float
+            Heliocentric redshift of SN to be used when fitting
+        ebv_mw: float, optional
+            Milky Way E(B-V) value of SN. Defaults to 0.
+        peak_mjd: float or Boolean, optional
+            Fiducial value for maximum MJD of SN, used to convert phases to rest-frame. Note that this value only needs
+            to be rough as BayeSN will fit for the time of maximum. However, if you set fix_tmax=True then this will
+            be fixed as the time of maximum. Defaults to False, meaning that the code will assume phases are already
+            rest-frame rather than MJD and will not do any conversion
+        filt_map: dict, optional
+            Dictionary providing mapping between filter names in file and BayeSN filters. Defaults to empty dictionary
+        print_summary: Boolean, optional
+            Specifies whether to print fit summary
+        file_prefix: str, optional
+            Prefix of name for output files containing summary table and MCMC samples. Default to None, in which case
+            output files will not be saved and only returned for use in script.
+        drop_bands: array-like, optional
+            List of bands to be ignored during fitting. Defaults to empty list
+        fix_tmax: Boolean, optional
+            If True, tmax will not be inferred and fiducial value in file meta will be fixed. Defaults to False.
+        fix_theta: float, optional
+            Value to fix theta at during fitting. Defaults to False, meaning that theta will be inferred during fitting
+            rather than fixed.
+        fix_AV: float, optional
+            Value to fix AV at during fitting. Defaults to False, meaning that AV will be inferred during fitting
+            rather than fixed.
+        RV: float, optional
+            Value to fix RV at during fitting. Defaults to False, meaning that default model RV treatment will be used.
+        mu_R: float, optional
+            Value of mean of RV distribution to be used during fitting. Defaults to False, meaning that default model
+            RV treatment will be used. If specified, sigma_R must also be specified.
+        sigma_R: float, optional
+            Value of standard deviation of RV distribution. Defaults to False, meaning that default model RV treatment
+            will be used.
+        mag: Boolean, optional
+            Specifies whether data is mag or flux. If True, data is assumed to be mag and is automatically converted to
+            flux before fitting.
+
+        Returns
+        -------
+
+        samples: dict
+            Dictionary containing parameter names as keys and MCMC samples as values
+        sn_props: tuple
+            Tuple containing SN redshift and MW E(B-V), which can be useful to have in memory when making plots
+
+        """
+        if type(drop_bands) == str:
+            drop_bands = [drop_bands]
+        t, flux, flux_err, filters = np.array(t), np.array(flux), np.array(flux_err), np.array(filters)
+        if mag:  # Convert data from mag into FLUXCAL
+            flux = np.power(10, (27.5 - flux) / 2.5)
+            flux_err = (np.log(10) / 2.5) * flux * flux_err
+        if peak_mjd is not None:
+            t = (t - peak_mjd) / (1 + z)
+        flux = flux[(t > self.tau_knots.min()) & (t < self.tau_knots.max())]
+        flux_err = flux_err[(t > self.tau_knots.min()) & (t < self.tau_knots.max())]
+        filters = filters[(t > self.tau_knots.min()) & (t < self.tau_knots.max())]
+        filters = np.array([filt_map.get(filter, filter) for filter in filters])
+        t = t[(t > self.tau_knots.min()) & (t < self.tau_knots.max())]
+
+        # Prepare filters
+        for f in np.unique(filters):
+            if f not in self.band_dict.keys():
+                raise ValueError(f'Filter "{filter}" not defined in BayeSN, either add a mapping to filt_map to ensure '
+                                 f'that your filter names match up with ones built-in or add some custom filters if '
+                                 f'you want to use your own')
+            if z > (self.band_lim_dict[f][0] / self.l_knots[0] - 1) or z < (
+                    self.band_lim_dict[f][1] / self.l_knots[-1] - 1):
+                drop_bands.append(f)
+        for f in drop_bands:
+            inds = filters != f
+            flux = flux[inds]
+            flux_err = flux_err[inds]
+            filters = filters[inds]
+            t = t[inds]
+        band_indices = np.array([self.band_dict[filt_map.get(filter, filter)] for filter in filters])
+
+        n_data = len(t)
+        if n_data == 0:
+            raise ValueError('No data in rest-frame phase range covered by model, maybe you gave the wrong peak MJD?')
+        # Set up and populate data array
+        data = jnp.zeros((10, n_data, 1))
+        data = data.at[0, :, 0].set(t)
+        data = data.at[1, :, 0].set(flux)
+        data = data.at[2, :, 0].set(flux_err)
+        data = data.at[4, :, 0].set(band_indices)
+        data = data.at[5, :, 0].set(np.full_like(t, z))
+        data = data.at[7, :, 0].set(np.full_like(t, self.cosmo.distmod(z).value))
+        data = data.at[8, :, 0].set(np.full_like(t, ebv_mw))
+        data = data.at[9, :, 0].set(np.ones_like(t))
+
+        band_weights = self._calculate_band_weights(data[-5, 0, :], data[-2, 0, :])
+
+        # Update dust parameters if specified manually
+        if RV:
+            self.RV = jnp.array(RV)
+            self.model_type = 'fixed_RV'
+        elif mu_R:
+            if not sigma_R:
+                raise ValueError('You have set a custom mu_R, please also set a custom sigma_R')
+            self.mu_R = jnp.array(mu_R)
+            self.sigma_R = jnp.array(sigma_R)
+            self.model_type = 'pop_RV'
+        if self.model_type == 'fixed_RV':
+            nuts_kernel = NUTS(self.fit_model_globalRV, adapt_step_size=True, init_strategy=init_to_median(),
+                               max_tree_depth=10)
+        elif self.model_type == 'pop_RV':
+            nuts_kernel = NUTS(self.fit_model_popRV, adapt_step_size=True, init_strategy=init_to_median(),
+                               max_tree_depth=10)
+        mcmc = MCMC(nuts_kernel, num_samples=250, num_warmup=250, num_chains=4, chain_method='parallel')
         rng = PRNGKey(0)
-        start = timeit.default_timer()
-        # self.data, self.band_weights = self.data[..., 0:2], self.band_weights[0:2, ...]
-        # print(self.data.shape)
-        mcmc.run(rng, self.data, self.band_weights, extra_fields=('potential_energy',))
-        end = timeit.default_timer()
-        print(f'Total HMC runtime: {end - start} seconds')
-        mcmc.print_summary()
+
+        theta_val = 0
+        if fix_theta:
+            theta_val = fix_theta
+            fix_theta = True
+        AV_val = 0
+        if fix_AV:
+            AV_val = fix_AV
+            fix_AV = True
+
+        mcmc.run(rng, data, band_weights, fix_tmax, fix_theta, theta_val, fix_AV, AV_val,
+                 extra_fields=('potential_energy',))
+        if print_summary:
+            mcmc.print_summary()
         samples = mcmc.get_samples(group_by_chain=True)
-        self.postprocess(samples, args)
+        if peak_mjd is not None:
+            samples['peak_MJD'] = peak_mjd + samples['tmax'] * (1 + z)
+        muhat = self.cosmo.distmod(z).value
+        muhat_err = 5
+        Ds_err = jnp.sqrt(muhat_err * muhat_err + self.sigma0 * self.sigma0)
+        samples['mu'] = np.random.normal((samples['Ds'] * np.power(muhat_err, 2) + muhat * np.power(self.sigma0, 2)) /
+            np.power(Ds_err, 2), np.sqrt((np.power(self.sigma0, 2) * np.power(muhat_err, 2)) / np.power(Ds_err, 2)))
+        samples['delM'] = samples['Ds'] - samples['mu']
+        if fix_tmax:
+            samples['tmax'] = jnp.zeros_like(samples['tmax'])
+        if fix_theta:
+            samples['theta'] = jnp.full_like(samples['theta'], theta_val)
+        if fix_AV:
+            samples['AV'] = jnp.full_like(samples['AV'], AV_val)
+
+        if file_prefix is not None:
+            summary = arviz.summary(samples)
+            summary.to_csv(f'{file_prefix}_fit_summary.csv')
+            with open(f'{file_prefix}_chains.pkl', 'wb') as file:
+                pickle.dump(samples, file)
+
+        sn_props = (z, ebv_mw)
+
+        return samples, sn_props
 
     def postprocess(self, samples, args):
         """
         Function to postprocess BayeSN output. Applies transformations to some parameters e.g. ensuring consistency for
         W1 and theta, as flipping the sign in front of W1 and theta will lead to an identical result. Saves output
         chains and calculated a fit summary
 
@@ -1651,14 +2155,17 @@
             muhat_err = 5
             Ds_err = jnp.sqrt(muhat_err * muhat_err + self.sigma0 * self.sigma0)
             samples['mu'] = np.random.normal(
                 (samples['Ds'] * np.power(muhat_err, 2) + muhat * np.power(self.sigma0, 2)) /
                 np.power(Ds_err, 2),
                 np.sqrt((np.power(self.sigma0, 2) * np.power(muhat_err, 2)) / np.power(Ds_err, 2)))
             samples['delM'] = samples['Ds'] - samples['mu']
+            if 'tmax' in samples.keys():  # Convert tmax samples into peak_MJD samples
+                samples['peak_MJD'] = self.peak_mjds[None, None, :] + samples['tmax'] * (
+                            1 + z_HEL[None, None, :])
 
             # Create FITRES file
             if args['snana']:
                 # fetch snana version that includes tag + commit;
                 # e.g., v11_05-4-gd033611.
                 # Use same git command as in Makefile for C code
                 SNANA_DIR = os.environ.get('SNANA_DIR', 'NULL')
@@ -1669,43 +2176,50 @@
                 else:
                     snana_version = 'NULL'
                 self.fitres_table.meta = {'#\n# SNANA_VERSION:': snana_version,
                                           '# VERSION_PHOTOMETRY:': args['version_photometry'],
                                           '# TABLE NAME:': 'FITRES\n#'}
 
                 n_sn = samples['mu'].shape[-1]
+                drop_keys = ['diverging', '_auto_latent']
+                for key in drop_keys:
+                    if key in samples.keys():
+                        del samples[key]
                 summary = arviz.summary(samples)
                 summary = summary[~summary.index.str.contains('tform')]
                 rhat = summary.r_hat.values
                 sn_rhat = np.array([rhat[i::n_sn] for i in range(n_sn)])
 
                 self.fitres_table['MU'] = samples['mu'].mean(axis=(0, 1))
-                self.fitres_table['MU_ERR'] = samples['mu'].std(axis=(0, 1))
-                self.fitres_table['THETA_1'] = samples['theta'].mean(axis=(0, 1))
-                self.fitres_table['THETA_1_ERR'] = samples['theta'].std(axis=(0, 1))
+                self.fitres_table['MUERR'] = samples['mu'].std(axis=(0, 1))
+                self.fitres_table['THETA'] = samples['theta'].mean(axis=(0, 1))
+                self.fitres_table['THETAERR'] = samples['theta'].std(axis=(0, 1))
                 self.fitres_table['AV'] = samples['AV'].mean(axis=(0, 1))
-                self.fitres_table['AV_ERR'] = samples['AV'].std(axis=(0, 1))
-                self.fitres_table['MEAN_RHAT'] = sn_rhat.mean(axis=1)
-                self.fitres_table['MAX_RHAT'] = sn_rhat.max(axis=1)
+                self.fitres_table['AVERR'] = samples['AV'].std(axis=(0, 1))
+                # if not args['fit_method'] == 'vi':
+                self.fitres_table['MEANRHAT'] = sn_rhat.mean(axis=1)
+                self.fitres_table['MAXRHAT'] = sn_rhat.max(axis=1)
                 self.fitres_table.round(3)
 
-                sncosmo.write_lc(self.fitres_table, f'{args["outfile_prefix"]}.FITRES.TEXT', fmt="snana",
-                                 metachar="")
+                drop_count = pd.isna(self.fitres_table['MU']).sum()
+                self.fitres_table = self.fitres_table[~pd.isna(self.fitres_table['MU'])]
+
+                sncosmo.write_lc(self.fitres_table, f'{args["outfile_prefix"]}.FITRES.TEXT', fmt="snana", metachar="")
 
         if args['snana']:
             self.end_time = time.time()
             cpu_time = self.end_time - self.start_time
             # Output yaml
             out_dict = {
                 'ABORT_IF_ZERO': 1,
                 'SURVEY': self.survey,
                 'IDSURVEY': int(self.survey_id),
                 'NEVT_TOT': self.data.shape[-1],
                 'NEVT_LC_CUTS': self.data.shape[-1],
-                'NEVT_LCFIT_CUTS': self.data.shape[-1],
+                'NEVT_LCFIT_CUTS': int(self.data.shape[-1] - drop_count),
                 'CPU_MINUTES': round(cpu_time / 60, 2),
             }
             with open(f'{args["outfile_prefix"]}.YAML', 'w') as file:
                 yaml.dump(out_dict, file)
 
         if not (args['mode'] == 'fitting' and args['snana']):
             # Save convergence data for each parameter to csv file
@@ -1783,15 +2297,15 @@
             list_file = os.path.join(data_dir, f'{os.path.split(data_dir)[-1]}.LIST')
             sn_list = np.atleast_1d(np.loadtxt(list_file, dtype='str'))
             file_format = sn_list[0].split('.')[1]
             map_dict = args['map']
             n_obs = []
             all_lcs = []
             t_ranges = []
-            sne = []
+            sne, peak_mjds = [], []
             # For FITRES table
             idsurvey, sn_type, field, cutflag_snana, z_hels, z_hel_errs, z_hds, z_hd_errs = [], [], [], [], [], [], [], []
             snrmax1s, snrmax2s, snrmax3s = [], [], []
             vpecs, vpec_errs, mwebvs, host_logmasses, host_logmass_errs = [], [], [], [], []
             # --------
             used_bands, used_band_dict = ['NULL_BAND'], {0: 0}
             print('Reading light curves...')
@@ -1820,14 +2334,15 @@
                         ntot += 1
                         if (ntot - args['jobid']) % args['njobtot'] != 0:
                             continue
                         sn = sne_file[sn_ind]
                         meta, data = sn.meta, sn.to_pandas()
                         data['BAND'] = data.BAND.str.decode("utf-8")
                         data['BAND'] = data.BAND.str.strip()
+                        data = data[data.BAND == 'z']
                         peak_mjd = meta['PEAKMJD']
                         zhel = meta['REDSHIFT_HELIO']
                         zcmb = meta['REDSHIFT_FINAL']
                         zhel_err = 5e-4  # Need to handle this better if not defined
                         zcmb_err = 5e-4  # Need to handle this better if not defined
                         data['t'] = (data.MJD - peak_mjd) / (1 + zhel)
                         # If filter not in map_dict, assume one-to-one mapping------
@@ -1874,14 +2389,15 @@
                         all_lcs.append(lc)
                         # Set up FITRES table data
                         # (currently just uses second table, should improve for cases where there are multiple lc files)
                         sn_name = meta['SNID']
                         if isinstance(sn_name, bytes):
                             sn_name = sn_name.decode('utf-8')
                         sne.append(sn_name)
+                        peak_mjds.append(peak_mjd)
                         sn_type.append(meta.get('TYPE', 0))
                         field.append(meta.get('FIELD', 'VOID'))
                         z_hels.append(zhel)
                         z_hel_errs.append(meta.get('REDSHIFT_HELIO_ERR', zhel_err))
                         z_hds.append(meta['REDSHIFT_FINAL'])
                         z_hd_errs.append(meta.get('REDSHIFT_FINAL_ERR', zcmb_err))
                         vpecs.append(meta.get('VPEC', 0.))
@@ -1917,15 +2433,14 @@
                         continue
                     meta, lcdata = sncosmo.read_snana_ascii(os.path.join(data_dir, sn_file), default_tablename='OBS')
                     data = lcdata['OBS'].to_pandas()
                     peak_mjd = meta['PEAKMJD']
                     sn_name = meta['SNID']
                     if isinstance(sn_name, bytes):
                         sn_name = sn_name.decode('utf-8')
-                    sne.append(sn_name)
                     zhel = meta['REDSHIFT_HELIO']
                     zcmb = meta['REDSHIFT_FINAL']
                     zhel_err = 5e-4  # Placeholder in case value is not defined in meta, need to handle this better
                     zcmb_err = 5e-4  # Placeholder in case value is not defined in meta, need to handle this better
                     data['t'] = (data.MJD - peak_mjd) / (1 + zhel)
                     # If filter not in map_dict, assume one-to-one mapping------
                     map_dict = args['map']
@@ -1962,14 +2477,16 @@
                     data['dist_mod'] = self.cosmo.distmod(zcmb)
                     data['mask'] = 1
                     lc = data[
                         ['t', 'flux', 'flux_err', 'MAG', 'MAGERR', 'mass', 'band_indices', 'redshift', 'redshift_error',
                          'dist_mod', 'MWEBV', 'mask']]
                     lc = lc.dropna(subset=['flux', 'flux_err'])
                     lc = lc[(lc['t'] > self.tau_knots.min()) & (lc['t'] < self.tau_knots.max())]
+                    sne.append(sn_name)
+                    peak_mjds.append(peak_mjd)
                     t_ranges.append((lc['t'].min(), lc['t'].max()))
                     n_obs.append(lc.shape[0])
                     all_lcs.append(lc)
                     # Set up FITRES table data
                     # (currently just uses second table, should improve for cases where there are multiple lc files)
                     sn_type.append(meta.get('TYPE', 0))
                     field.append(meta.get('FIELD', 'VOID'))
@@ -2030,14 +2547,15 @@
                 self.data = device_put(flux_data)
             self.sn_list = sne
             self.J_t = device_put(J_t)
             self.used_band_inds = jnp.array([self.band_dict[f] for f in used_bands])
             self.zps = self.zps[self.used_band_inds]
             self.offsets = self.offsets[self.used_band_inds]
             self.band_weights = self._calculate_band_weights(self.data[-5, 0, :], self.data[-2, 0, :])
+            self.peak_mjds = np.array(peak_mjds)
             # Prep FITRES table
             varlist = ["SN:"] * len(sne)
             idsurvey = [self.survey_id] * len(sne)
             snrmax1s, snrmax2s, snrmax3s = np.array(snrmax1s), np.array(snrmax2s), np.array(snrmax3s)
             table = QTable([varlist, sne, idsurvey, sn_type, field, z_hels, z_hel_errs, z_hds, z_hd_errs,
                             vpecs, vpec_errs, mwebvs, host_logmasses, host_logmass_errs, snrmax1s, snrmax2s, snrmax3s],
                            names=['VARNAMES:', 'CID', 'IDSURVEY', 'TYPE', 'FIELD', 'zHEL', 'zHELERR',
@@ -2053,14 +2571,15 @@
             t_ranges = []
             # For FITRES table
             idsurvey, sn_type, field, cutflag_snana, z_hels, z_hel_errs, z_hds, z_hd_errs = [], [], [], [], [], [], [], []
             snrmax1s, snrmax2s, snrmax3s = [], [], []
             vpecs, vpec_errs, mwebvs, host_logmasses, host_logmass_errs = [], [], [], [], []
             # --------
             used_bands, used_band_dict = ['NULL_BAND'], {0: 0}
+            sne, peak_mjds = [], []
             print('Reading light curves...')
             for i in tqdm(range(sn_list.shape[0])):
                 row = sn_list.iloc[i]
                 sn_files = row.files.split(',')
                 sn_lc = None
                 sn = row.SNID
                 data_root = args['data_root']
@@ -2102,27 +2621,29 @@
                     data['zp'] = data.FLT.apply(lambda x: self.zp_dict[x])
                     data['MAG'] = 27.5 - 2.5 * np.log10(data['FLUXCAL'])
                     data['MAGERR'] = (2.5 / np.log(10)) * data['FLUXCALERR'] / data['FLUXCAL']
                     data['flux'] = data['FLUXCAL']
                     data['flux_err'] = data['FLUXCALERR']
                     data['redshift'] = zhel
                     data['redshift_error'] = row.REDSHIFT_CMB_ERR
-                    data['MWEBV'] = meta['MWEBV']
-                    data['mass'] = meta['HOSTGAL_LOGMASS']
+                    data['MWEBV'] = meta.get('MWEBV', 0.)
+                    data['mass'] = meta.get('HOSTGAL_LOGMASS', -9.)
                     data['dist_mod'] = self.cosmo.distmod(row.REDSHIFT_CMB)
                     data['mask'] = 1
                     lc = data[
                         ['t', 'flux', 'flux_err', 'MAG', 'MAGERR', 'mass', 'band_indices', 'redshift', 'redshift_error',
                          'dist_mod', 'MWEBV', 'mask']]
                     lc = lc.dropna(subset=['flux', 'flux_err'])
                     lc = lc[(lc['t'] > self.tau_knots.min()) & (lc['t'] < self.tau_knots.max())]
                     if sn_lc is None:
                         sn_lc = lc.copy()
                     else:
                         sn_lc = pd.concat([sn_lc, lc])
+                sne.append(sn)
+                peak_mjds.append(peak_mjd)
                 t_ranges.append((lc['t'].min(), lc['t'].max()))
                 n_obs.append(lc.shape[0])
                 all_lcs.append(sn_lc)
                 # Set up FITRES table data
                 # (currently just uses second table, should improve for cases where there are multiple lc files)
                 idsurvey.append(meta.get('IDSURVEY', 'NULL'))
                 sn_type.append(meta.get('TYPE', 'NULL'))
@@ -2135,17 +2656,25 @@
                 vpecs.append(meta.get('VPEC', 'NULL'))
                 vpec_errs.append(meta.get('VPEC_ERR', 'NULL'))
                 mwebvs.append(meta.get('MWEBV', 'NULL'))
                 host_logmasses.append(meta.get('HOSTGAL_LOGMASS', 'NULL'))
                 host_logmass_errs.append(meta.get('HOSTGAL_LOGMASS_ERR', 'NULL'))
                 snrmax1 = np.max(lc.flux / lc.flux_err)
                 lc_snr2 = lc[lc.band_indices != lc[(lc.flux / lc.flux_err) == snrmax1].band_indices.values[0]]
-                snrmax2 = np.max(lc_snr2.flux / lc_snr2.flux_err)
-                lc_snr3 = lc_snr2[lc_snr2.band_indices != lc_snr2[(lc_snr2.flux / lc_snr2.flux_err) == snrmax2].band_indices.values[0]]
-                snrmax3 = np.max(lc_snr3.flux / lc_snr3.flux_err)
+                if lc_snr2.shape[0] == 0:
+                    snrmax2 = -99
+                    snrmax3 = -99
+                else:
+                    snrmax2 = np.max(lc_snr2.flux / lc_snr2.flux_err)
+                    lc_snr3 = lc_snr2[lc_snr2.band_indices !=
+                                      lc_snr2[(lc_snr2.flux / lc_snr2.flux_err) == snrmax2].band_indices.values[0]]
+                    if lc_snr3.shape[0] == 0:
+                        snrmax3 = -99
+                    else:
+                        snrmax3 = np.max(lc_snr3.flux / lc_snr3.flux_err)
                 snrmax1s.append(snrmax1)
                 snrmax2s.append(snrmax2)
                 snrmax3s.append(snrmax3)
             N_sn = sn_list.shape[0]
             N_obs = np.max(n_obs)
             N_col = lc.shape[1]
             all_data = np.zeros((N_sn, N_obs, N_col))
@@ -2177,14 +2706,15 @@
             else:
                 self.data = device_put(flux_data)
             self.J_t = device_put(J_t)
             self.used_band_inds = jnp.array([self.band_dict[f] for f in used_bands])
             self.zps = self.zps[self.used_band_inds]
             self.offsets = self.offsets[self.used_band_inds]
             self.band_weights = self._calculate_band_weights(self.data[-5, 0, :], self.data[-2, 0, :])
+            self.peak_mjds = np.array(peak_mjds)
 
             # Prep FITRES table
             varlist = ["SN:"] * len(sne)
             snrmax1s, snrmax2s, snrmax3s = np.array(snrmax1s), np.array(snrmax2s), np.array(snrmax3s)
             snrmax1s, snrmax2s, snrmax3s = np.around(snrmax1s, 2), np.around(snrmax2s, 2), np.around(snrmax3s, 2)
             table = QTable([varlist, sne, idsurvey, sn_type, field, z_hels, z_hel_errs, z_hds, z_hd_errs,
                             vpecs, vpec_errs, mwebvs, host_logmasses, host_logmass_errs, snrmax1s, snrmax2s, snrmax3s],
@@ -2366,15 +2896,15 @@
         mw_ext = np.zeros((N, l_o.shape[1], 1))
         for i in range(N):
             mw_ext[i, :, 0] = extinction.fitzpatrick99(l_o[i, ...], 3.1 * ebv_mw[i], 3.1)
 
         return l_o, spectra, param_dict
 
     def simulate_light_curve(self, t, N, bands, yerr=0, err_type='mag', z=0, zerr=1e-4, mu=0, ebv_mw=0, RV=None,
-                             logM=None, del_M=None, AV=None, theta=None, eps=None, mag=True, write_to_files=False,
+                             logM=None, tmax=0, del_M=None, AV=None, theta=None, eps=None, mag=True, write_to_files=False,
                              output_dir=None):
         """
         Simulates light curves from the BayeSN model in either mag or flux space. and saves them to SNANA-format text
         files if requested
 
         Parameters
         ----------
@@ -2414,14 +2944,18 @@
         RV: float or array-like, optional
             RV values for host extinction curves for simulated spectra. If passing an array-like object, there must be a
             corresponding value for each of the N simulated objects. If a float is passed, the same value will be used
             for all objects. Defaults to None, in which case the global RV value for the BayeSN model loaded when
             initialising SEDmodel will be used.
         logM: float or array-like, optional
             Currently unused, will be implemented when split models are included
+        tmax: float or array-like, optional
+            Time of maximum in rest-frame days, useful for plotting light curve fits with free tmax. Defaults to 0, i.e.
+            the simulated time of maximum will be at 0 days. If a float is passed, the same value will be used
+            for all objects.
         del_M: float or array-like, optional
             Grey offset del_M value to be used for each SN. If passing an array-like object, there must be a
             corresponding value for each of the N simulated objects. If a float is passed, the same value will be used
             for all objects. Defaults to None, in which case the prior distribution will be sampled for each object.
         AV: float or array-like, optional
             Host extinction RV value to be used for each SN. If passing an array-like object, there must be a
             corresponding value for each of the N simulated objects. If a float is passed, the same value will be used
@@ -2495,14 +3029,20 @@
             raise ValueError('For epsilon, please pass an array-like object of shape (N, l_knots, tau_knots)')
         ebv_mw = np.array(ebv_mw)
         if len(ebv_mw.shape) == 0:
             ebv_mw = ebv_mw.repeat(N)
         elif ebv_mw.shape[0] != N:
             raise ValueError(
                 'For ebv_mw, either pass a single scalar value or an array of values for each of the N simulated objects')
+        tmax = np.array(tmax)
+        if len(tmax.shape) == 0:
+            tmax = tmax.repeat(N)
+        elif tmax.shape[0] != N:
+            raise ValueError('If not providing a scalar tmax value, array must be of same length as the number of '
+                             'objects to simulate, N')
         if RV is None:
             RV = self.RV
         RV = np.array(RV)
         if len(RV.shape) == 0:
             RV = RV.repeat(N)
         elif RV.shape[0] != N:
             raise ValueError(
@@ -2547,14 +3087,15 @@
                     raise ValueError(f'{band} is present in filters yaml file')
                 band_indices[i * num_per_band: (i + 1) * num_per_band] = self.band_dict[band]
             band_indices = band_indices[:, None].repeat(N, axis=1).astype(int)
         mask = np.ones_like(band_indices)
         band_weights = self._calculate_band_weights(z, ebv_mw)
 
         t = jnp.repeat(t[..., None], N, axis=1)
+        t = t - tmax[None, :]
         hsiao_interp = jnp.array([19 + jnp.floor(t), 19 + jnp.ceil(t), jnp.remainder(t, 1)])
         keep_shape = t.shape
         t = t.flatten(order='F')
         map = jax.vmap(self.spline_coeffs_irr_step, in_axes=(0, None, None))
         J_t = map(t, self.tau_knots, self.KD_t).reshape((*keep_shape, self.tau_knots.shape[0]), order='F').transpose(1,
                                                                                                                      2,
                                                                                                                      0)
@@ -2674,15 +3215,15 @@
         eps_tform = eps_tform.T
         eps = np.matmul(self.L_Sigma, eps_tform)
         eps = np.reshape(eps, (N, self.l_knots.shape[0] - 2, self.tau_knots.shape[0]), order='F')
         eps_full = np.zeros((N, self.l_knots.shape[0], self.tau_knots.shape[0]))
         eps_full[:, 1:-1, :] = eps
         return eps_full
 
-    def get_flux_from_chains(self, t, bands, chain_path, zs, ebv_mws, mag=True, num_samples=None):
+    def get_flux_from_chains(self, t, bands, chains, zs, ebv_mws, mag=True, num_samples=None):
         """
         Returns model photometry for posterior samples from BayeSN fits, which can be used to make light curve fit
         plots.
 
         Parameters
         ----------
         t: array-like
@@ -2709,27 +3250,34 @@
         -------
 
         flux_grid: jax.numpy.array
             Array of shape (number of SNe, number of posterior samples, number of bands, number of phases to evaluate),
             containing photometry across all SNe, all posterior samples, all bands and at all phases requested.
 
         """
-        with open(chain_path, 'rb') as file:
-            chains = pickle.load(file)
+        if type(chains) == str:
+            with open(chains, 'rb') as file:
+                chains = pickle.load(file)
 
         N_sne = chains['theta'].shape[2]
         if num_samples is None:
             num_samples = chains['theta'].shape[0] * chains['theta'].shape[1]
 
+        if isinstance(zs, float):
+            zs = np.array([zs])
+        if isinstance(ebv_mws, float):
+            ebv_mws = np.array([ebv_mws])
+
         flux_grid = jnp.zeros((N_sne, num_samples, len(bands), len(t)))
 
         print('Getting best fit light curves from chains...')
         for i in tqdm(np.arange(N_sne)):
             theta = chains['theta'][..., i].flatten(order='F')
             AV = chains['AV'][..., i].flatten(order='F')
+            tmax = chains['tmax'][..., i].flatten(order='F')
             if 'RV' in chains.keys():
                 RV = chains['RV'][..., i].flatten(order='F')
             else:
                 RV = None
             mu = chains['mu'][..., i].flatten(order='F')
             eps = chains['eps'][..., i]
             eps = eps.reshape((eps.shape[0] * eps.shape[1], eps.shape[2]), order='F')
@@ -2737,15 +3285,15 @@
             eps_full = jnp.zeros((eps.shape[0], self.l_knots.shape[0], self.tau_knots.shape[0]))
             eps = eps_full.at[:, 1:-1, :].set(eps)
             del_M = chains['delM'][..., i].flatten(order='F')
 
             theta, AV, mu, eps, del_M = theta[:num_samples], AV[:num_samples], mu[:num_samples], \
                                         eps[:num_samples, ...], del_M[:num_samples, ...]
 
-            lc, lc_err, params = self.simulate_light_curve(t, num_samples, bands, theta=theta, AV=AV, mu=mu,
+            lc, lc_err, params = self.simulate_light_curve(t, num_samples, bands, theta=theta, AV=AV, mu=mu, tmax=tmax,
                                                            del_M=del_M, eps=eps, RV=RV, z=zs[i], write_to_files=False,
                                                            ebv_mw=ebv_mws[i], yerr=0, mag=mag)
             lc = lc.T
             lc = lc.reshape(num_samples, len(bands), len(t))
-            flux_grid.at[i, ...].set(lc)
+            flux_grid = flux_grid.at[i, ...].set(lc)
 
         return flux_grid
```

### Comparing `bayesn-0.3.2/bayesn/data/hsiao.h5` & `bayesn-0.4.0/bayesn/data/hsiao.h5`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/model_files/M20_model/BAYESN.INFO` & `bayesn-0.4.0/bayesn/model_files/M20_model/BAYESN.INFO`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/model_files/M20_model/BAYESN.YAML` & `bayesn-0.4.0/bayesn/model_files/M20_model/BAYESN.YAML`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/model_files/README.md` & `bayesn-0.4.0/bayesn/model_files/README.md`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/model_files/T21_model/BAYESN.INFO` & `bayesn-0.4.0/bayesn/model_files/T21_model/BAYESN.INFO`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/model_files/T21_model/BAYESN.YAML` & `bayesn-0.4.0/bayesn/model_files/T21_model/BAYESN.YAML`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/model_files/W22_model/BAYESN.INFO` & `bayesn-0.4.0/bayesn/model_files/W22_model/BAYESN.INFO`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/model_files/W22_model/BAYESN.YAML` & `bayesn-0.4.0/bayesn/model_files/W22_model/BAYESN.YAML`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn/spline_utils.py` & `bayesn-0.4.0/bayesn/spline_utils.py`

 * *Files identical despite different names*

### Comparing `bayesn-0.3.2/bayesn.egg-info/PKG-INFO` & `bayesn-0.4.0/bayesn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesn
-Version: 0.3.2
+Version: 0.4.0
 Summary: Hierarchical Bayesian modelling of type Ia SNe
 Home-page: https://github.com/bayesn/bayesn
 Author: Matt Grayling, Stephen Thorp, Kaisey Mandel
 Author-email: mg2102@cam.ac.uk
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,15 +35,15 @@
 Developed and maintained by: Matt Grayling (@mattgrayling), Stephen Thorp (@stevet40), Gautham Narayan (@gnarayan), and 
 Kaisey S. Mandel (@CambridgeAstroStat) on behalf of the BayeSN Team (@bayesn).
 
 ## About
 BayeSN is a probabilistic optical-NIR SED model for type Ia supernovae, allowing for hierarchical analysis of the
 population distribution of physical properties as well as cosmology-independent distance estimation for individual
 SNe. This repository contains an implementation of the BayeSN SED model built with numpyro and jax, with support for 
-GPU acceleration, as discussed in Grayling+2024 (submitted to MNRAS).
+GPU acceleration, as discussed in Grayling+2024 (`arXiv link <https://arxiv.org/abs/2401.08755>`, accepted by MNRAS).
 
 ## Installation and usage
 BayeSN can be pip-installed via the command `pip install bayesn`. 
 
 Detailed instructions on how to install and run the BayeSN model can be found here: https://bayesn.readthedocs.io/en/latest/index.html
 
 ## Support
```

### Comparing `bayesn-0.3.2/bayesn.egg-info/SOURCES.txt` & `bayesn-0.4.0/bayesn.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 run_bayesn
 setup.cfg
 setup.py
 bayesn/__init__.py
 bayesn/bayesn_io.py
 bayesn/bayesn_model.py
 bayesn/spline_utils.py
+bayesn/zltn_utils.py
 bayesn.egg-info/PKG-INFO
 bayesn.egg-info/SOURCES.txt
 bayesn.egg-info/dependency_links.txt
 bayesn.egg-info/requires.txt
 bayesn.egg-info/top_level.txt
 bayesn/bayesn-filters/filters.yaml
 bayesn/bayesn-filters/filters/CTIO/ANDICAM/Bandicam.dat
@@ -83,14 +84,20 @@
 bayesn/bayesn-filters/filters/LCO/Swope/u_tel_ccd_atm_ext_1.2.dat
 bayesn/bayesn-filters/filters/LSST/total_g.dat
 bayesn/bayesn-filters/filters/LSST/total_i.dat
 bayesn/bayesn-filters/filters/LSST/total_r.dat
 bayesn/bayesn-filters/filters/LSST/total_u.dat
 bayesn/bayesn-filters/filters/LSST/total_y.dat
 bayesn/bayesn-filters/filters/LSST/total_z.dat
+bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_g.dat
+bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_i.dat
+bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_r.dat
+bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_u.dat
+bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_y.dat
+bayesn/bayesn-filters/filters/LSST/2017-04_approx/LSST_z.dat
 bayesn/bayesn-filters/filters/NULL/NULL.dat
 bayesn/bayesn-filters/filters/PS1/g_filt_revised.txt
 bayesn/bayesn-filters/filters/PS1/g_filt_tonry.txt
 bayesn/bayesn-filters/filters/PS1/i_filt_tonry.txt
 bayesn/bayesn-filters/filters/PS1/r_filt_tonry.txt
 bayesn/bayesn-filters/filters/PS1/y_filt_tonry.txt
 bayesn/bayesn-filters/filters/PS1/z_filt_tonry.txt
@@ -124,14 +131,15 @@
 bayesn/bayesn-filters/filters/standard/stritzinger/i_stritzinger
 bayesn/bayesn-filters/filters/standard/stritzinger/r_stritzinger
 bayesn/bayesn-filters/filters/standard/stritzinger/u_stritzinger
 bayesn/bayesn-filters/filters/standard/stritzinger/v_stritzinger
 bayesn/bayesn-filters/standards/alpha_lyr_stis_010.fits
 bayesn/bayesn-filters/standards/bd_17d4708_stisnic_007.dat
 bayesn/data/hsiao.h5
+bayesn/data/example_lcs/Foundation_DR1_2016W.txt
 bayesn/model_files/README.md
 bayesn/model_files/M20_model/BAYESN.INFO
 bayesn/model_files/M20_model/BAYESN.YAML
 bayesn/model_files/T21_model/BAYESN.INFO
 bayesn/model_files/T21_model/BAYESN.YAML
 bayesn/model_files/W22_model/BAYESN.INFO
 bayesn/model_files/W22_model/BAYESN.YAML
```

### Comparing `bayesn-0.3.2/docs/conf.py` & `bayesn-0.4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'bayesn'
 copyright = '2023, Matthew Grayling, Stephen Thorp, Kaisey Mandel'
 author = 'Matthew Grayling, Stephen Thorp, Kaisey Mandel'
-release = '0.3.2'
+release = '0.4.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['numpydoc', 'sphinx.ext.autosummary', 'sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `bayesn-0.3.2/run_bayesn` & `bayesn-0.4.0/run_bayesn`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 parser = argparse.ArgumentParser()
 parser.add_argument('input', type=str)
 parser.add_argument('--filters', type=str, required=False)
 parser.add_argument('--outputdir', type=str, required=False)
 parser.add_argument('--load_model', type=str, required=False)
 parser.add_argument('--mode', type=str, required=False)
 parser.add_argument('--num_chains', type=int, required=False)
+parser.add_argument('--fit_method', type=str, required=False)
 parser.add_argument('--chain_method', type=str, required=False)
 parser.add_argument('--initialisation', type=str, required=False)
 parser.add_argument('--l_knots', type=float, required=False, nargs='*')
 parser.add_argument('--tau_knots', type=float, required=False, nargs='*')
 parser.add_argument('--map', type=str, required=False)
 parser.add_argument('--data_root', type=str, required=False)
 parser.add_argument('--data_table', type=str, required=False)
```

### Comparing `bayesn-0.3.2/setup.cfg` & `bayesn-0.4.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bayesn
-version = 0.3.2
+version = 0.4.0
 author = Matt Grayling, Stephen Thorp, Kaisey Mandel
 author_email = mg2102@cam.ac.uk
 description = Hierarchical Bayesian modelling of type Ia SNe
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bayesn/bayesn
 
@@ -26,27 +26,29 @@
 	ruamel.yaml
 	tqdm
 scripts = 
 	run_bayesn
 include_package_data = True
 
 [options.package_data]
-bayesn = bayesn/data/hsiao.h5
+bayesn = bayesn/data/*
+	bayesn/data/example_lcs/*
 	bayesn/bayesn-filters/*
 	bayesn/bayesn-filters/filters/*
 	bayesn/bayesn-filters/filters/CTIO/*
 	bayesn/bayesn-filters/filters/CTIO/ANDICAM/*
 	bayesn/bayesn-filters/filters/DECam/*
 	bayesn/bayesn-filters/filters/HST/WFC3/*
 	bayesn/bayesn-filters/filters/HST/WFC3/IR/*
 	bayesn/bayesn-filters/filters/HST/WFC3/UVIS2/*
 	bayesn/bayesn-filters/filters/LCO/*
 	bayesn/bayesn-filters/filters/LCO/Dupont/*
 	bayesn/bayesn-filters/filters/LCO/Swope/*
 	bayesn/bayesn-filters/filters/LSST/*
+	bayesn/bayesn-filters/filters/LSST/2017-04_approx/*
 	bayesn/bayesn-filters/filters/NULL/*
 	bayesn/bayesn-filters/filters/PS1/*
 	bayesn/bayesn-filters/filters/standard/*
 	bayesn/bayesn-filters/filters/standard/2MASS_PAIRITEL/*
 	bayesn/bayesn-filters/filters/standard/Persson/*
 	bayesn/bayesn-filters/filters/standard/stritzinger/*
 	bayesn/bayesn-filters/filters/Swift/*
```

