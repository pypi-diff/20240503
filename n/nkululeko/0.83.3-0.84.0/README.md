# Comparing `tmp/nkululeko-0.83.3.tar.gz` & `tmp/nkululeko-0.84.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.83.3.tar", last modified: Tue Apr 30 09:48:46 2024, max compression
+gzip compressed data, was "nkululeko-0.84.0.tar", last modified: Fri May  3 14:50:51 2024, max compression
```

## Comparing `nkululeko-0.83.3.tar` & `nkululeko-0.84.0.tar`

### file list

```diff
@@ -1,224 +1,225 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.447454 nkululeko-0.83.3/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17539 2024-04-30 09:39:09.000000 nkululeko-0.83.3/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.83.3/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36267 2024-04-30 09:48:46.447454 nkululeko-0.83.3/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.83.3/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.83.3/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.83.3/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.83.3/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.83.3/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.83.3/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.83.3/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.83.3/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.83.3/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.83.3/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.83.3/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.83.3/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.83.3/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.83.3/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.83.3/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.83.3/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.83.3/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.83.3/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.83.3/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.83.3/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.83.3/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.83.3/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.83.3/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.83.3/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.83.3/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.83.3/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.83.3/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.439454 nkululeko-0.83.3/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.439454 nkululeko-0.83.3/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.83.3/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.439454 nkululeko-0.83.3/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.83.3/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.439454 nkululeko-0.83.3/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.83.3/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.439454 nkululeko-0.83.3/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.83.3/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.439454 nkululeko-0.83.3/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.83.3/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.439454 nkululeko-0.83.3/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.83.3/meta/demos/demo_best_model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.83.3/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.83.3/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.83.3/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.439454 nkululeko-0.83.3/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.83.3/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.83.3/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.83.3/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.439454 nkululeko-0.83.3/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.83.3/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.83.3/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.83.3/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.83.3/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.83.3/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.443454 nkululeko-0.83.3/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.83.3/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.83.3/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.83.3/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.83.3/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-30 09:39:44.000000 nkululeko-0.83.3/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.443454 nkululeko-0.83.3/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.83.3/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.83.3/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.83.3/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3264 2024-04-22 09:09:10.000000 nkululeko-0.83.3/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.83.3/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4755 2024-04-22 09:09:10.000000 nkululeko-0.83.3/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29873 2024-04-30 09:37:37.000000 nkululeko-0.83.3/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2310 2024-04-22 09:09:10.000000 nkululeko-0.83.3/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.83.3/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.443454 nkululeko-0.83.3/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.83.3/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_auddim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4576 2024-04-29 13:37:24.000000 nkululeko-0.83.3/nkululeko/feat_extract/feats_whisper.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.83.3/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.83.3/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.83.3/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.83.3/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.83.3/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.83.3/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.443454 nkululeko-0.83.3/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.83.3/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.83.3/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.83.3/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9288 2024-04-25 13:02:38.000000 nkululeko-0.83.3/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.443454 nkululeko-0.83.3/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.83.3/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11569 2024-04-17 13:01:47.000000 nkululeko-0.83.3/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.83.3/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10002 2024-04-29 13:37:24.000000 nkululeko-0.83.3/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.83.3/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.83.3/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.83.3/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.83.3/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9471 2024-04-29 13:37:24.000000 nkululeko-0.83.3/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10290 2024-04-29 13:37:24.000000 nkululeko-0.83.3/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      914 2024-04-17 12:17:54.000000 nkululeko-0.83.3/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.83.3/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.83.3/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.83.3/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.83.3/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.83.3/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.83.3/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.83.3/nkululeko/nkuluflag.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.83.3/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.83.3/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.83.3/nkululeko/predict.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.443454 nkululeko-0.83.3/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.83.3/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.83.3/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.83.3/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.83.3/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.83.3/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.83.3/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.83.3/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2287 2024-04-22 09:09:10.000000 nkululeko-0.83.3/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.83.3/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.83.3/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.83.3/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.443454 nkululeko-0.83.3/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.83.3/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.83.3/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.83.3/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.83.3/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.83.3/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.83.3/nkululeko/test_predictor.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.447454 nkululeko-0.83.3/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.83.3/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.83.3/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.83.3/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.83.3/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.447454 nkululeko-0.83.3/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36267 2024-04-30 09:48:46.000000 nkululeko-0.83.3/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5073 2024-04-30 09:48:46.000000 nkululeko-0.83.3/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-30 09:48:46.000000 nkululeko-0.83.3/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-30 09:48:46.000000 nkululeko-0.83.3/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-30 09:48:46.000000 nkululeko-0.83.3/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.83.3/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-30 09:48:46.447454 nkululeko-0.83.3/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.83.3/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.435454 nkululeko-0.83.3/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-30 09:48:46.447454 nkululeko-0.83.3/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.83.3/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17618 2024-05-03 14:43:26.000000 nkululeko-0.84.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.84.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36346 2024-05-03 14:50:51.185131 nkululeko-0.84.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.84.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.149131 nkululeko-0.84.0/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.84.0/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.84.0/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.84.0/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.84.0/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.84.0/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.84.0/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.84.0/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.84.0/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.84.0/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.84.0/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.84.0/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.84.0/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.84.0/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.84.0/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.84.0/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.84.0/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.84.0/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.84.0/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.84.0/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.84.0/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.84.0/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.84.0/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.84.0/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.84.0/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.149131 nkululeko-0.84.0/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.84.0/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.149131 nkululeko-0.84.0/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.84.0/meta/demos/demo_best_model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.84.0/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.84.0/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.84.0/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.84.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.84.0/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.84.0/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.84.0/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.84.0/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.84.0/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.84.0/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.181131 nkululeko-0.84.0/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.84.0/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.84.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-03 14:50:26.000000 nkululeko-0.84.0/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.181131 nkululeko-0.84.0/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.84.0/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.84.0/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.84.0/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.84.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.84.0/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.84.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30225 2024-05-03 12:01:47.000000 nkululeko-0.84.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.84.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.84.0/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.181131 nkululeko-0.84.0/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.84.0/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_auddim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4576 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_whisper.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.84.0/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.84.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.84.0/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.84.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.84.0/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.181131 nkululeko-0.84.0/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.84.0/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.84.0/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.84.0/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9288 2024-04-25 13:02:38.000000 nkululeko-0.84.0/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.84.0/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11601 2024-05-03 14:31:11.000000 nkululeko-0.84.0/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.84.0/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.84.0/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.84.0/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.84.0/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.84.0/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.84.0/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9854 2024-05-03 14:29:13.000000 nkululeko-0.84.0/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.84.0/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.84.0/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.84.0/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.84.0/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.84.0/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.84.0/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.84.0/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.84.0/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.84.0/nkululeko/nkuluflag.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.84.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/predict.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.84.0/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.84.0/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.84.0/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.84.0/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.84.0/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.84.0/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2287 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.84.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.84.0/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.84.0/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.84.0/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.84.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.84.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.84.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3109 2024-05-03 14:39:48.000000 nkululeko-0.84.0/nkululeko/test_pretrain.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.84.0/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.84.0/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13068 2024-05-03 13:47:24.000000 nkululeko-0.84.0/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36346 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5100 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.84.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-03 14:50:51.185131 nkululeko-0.84.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.84.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.149131 nkululeko-0.84.0/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.84.0/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.83.3/CHANGELOG.md` & `nkululeko-0.84.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 0.84.0
+--------------
+* added SHAP analysis
+* started with finetuning
+
 Version 0.83.3
 --------------
 * fixed a naming error in trill features that prevented storage of experiment
 
 Version 0.83.2
 --------------
 * added default cuda if present and not stated
```

### Comparing `nkululeko-0.83.3/LICENSE` & `nkululeko-0.84.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/PKG-INFO` & `nkululeko-0.84.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.83.3
+Version: 0.84.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,19 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.84.0
+--------------
+* added SHAP analysis
+* started with finetuning
+
 Version 0.83.3
 --------------
 * fixed a naming error in trill features that prevented storage of experiment
 
 Version 0.83.2
 --------------
 * added default cuda if present and not stated
```

### Comparing `nkululeko-0.83.3/README.md` & `nkululeko-0.84.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/aesdd/process_database.py` & `nkululeko-0.84.0/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/androids/process_database.py` & `nkululeko-0.84.0/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/androids_orig/process_database.py` & `nkululeko-0.84.0/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/androids_test/process_database.py` & `nkululeko-0.84.0/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/ased/process_database.py` & `nkululeko-0.84.0/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/asvp-esd/process_database.py` & `nkululeko-0.84.0/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/baved/process_database.py` & `nkululeko-0.84.0/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/cafe/process_database.py` & `nkululeko-0.84.0/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/clac/process_database.py` & `nkululeko-0.84.0/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/cmu-mosei/process_database.py` & `nkululeko-0.84.0/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/demos/process_database.py` & `nkululeko-0.84.0/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/ekorpus/process_database.py` & `nkululeko-0.84.0/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/emns/process_database.py` & `nkululeko-0.84.0/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/emofilm/convert_to_16k.py` & `nkululeko-0.84.0/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/emofilm/process_database.py` & `nkululeko-0.84.0/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/emorynlp/process_database.py` & `nkululeko-0.84.0/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/emov-db/process_database.py` & `nkululeko-0.84.0/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/emovo/process_database.py` & `nkululeko-0.84.0/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/emozionalmente/create.py` & `nkululeko-0.84.0/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/enterface/process_database.py` & `nkululeko-0.84.0/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/esd/process_database.py` & `nkululeko-0.84.0/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/gerparas/process_database.py` & `nkululeko-0.84.0/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/iemocap/process_database.py` & `nkululeko-0.84.0/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/jl/process_database.py` & `nkululeko-0.84.0/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/jtes/process_database.py` & `nkululeko-0.84.0/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/meld/process_database.py` & `nkululeko-0.84.0/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/mesd/process_database.py` & `nkululeko-0.84.0/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/mess/process_database.py` & `nkululeko-0.84.0/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/mlendsnd/process_database.py` & `nkululeko-0.84.0/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/msp-improv/process_database2.py` & `nkululeko-0.84.0/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/msp-podcast/process_database.py` & `nkululeko-0.84.0/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/oreau2/process_database.py` & `nkululeko-0.84.0/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/portuguese/process_database.py` & `nkululeko-0.84.0/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/ravdess/process_database.py` & `nkululeko-0.84.0/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/ravdess/process_database_speaker.py` & `nkululeko-0.84.0/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/savee/process_database.py` & `nkululeko-0.84.0/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/shemo/process_database.py` & `nkululeko-0.84.0/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/subesco/process_database.py` & `nkululeko-0.84.0/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/tess/process_database.py` & `nkululeko-0.84.0/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/thorsten-emotional/process_database.py` & `nkululeko-0.84.0/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/urdu/process_database.py` & `nkululeko-0.84.0/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/data/vivae/process_database.py` & `nkululeko-0.84.0/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/docs/source/conf.py` & `nkululeko-0.84.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/meta/demos/demo_best_model.py` & `nkululeko-0.84.0/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/meta/demos/my_experiment.py` & `nkululeko-0.84.0/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/meta/demos/my_experiment_local.py` & `nkululeko-0.84.0/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/meta/demos/plot_faster_anim.py` & `nkululeko-0.84.0/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/aug_train.py` & `nkululeko-0.84.0/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/augment.py` & `nkululeko-0.84.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/augmenting/augmenter.py` & `nkululeko-0.84.0/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.84.0/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.84.0/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/augmenting/resampler.py` & `nkululeko-0.84.0/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_age.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.84.0/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.84.0/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/cacheddataset.py` & `nkululeko-0.84.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/data/dataset.py` & `nkululeko-0.84.0/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/data/dataset_csv.py` & `nkululeko-0.84.0/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/demo.py` & `nkululeko-0.84.0/nkululeko/demo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # demo.py
 # Demonstration code to use the ML-experiment framework
 # Test the loading of a previously trained model and demo mode
 # needs the project config file to run before
-"""
-This script is used to test the loading of a previously trained model and run it in demo mode.
+"""This script is used to test the loading of a previously trained model.
+
+And run it in demo mode.
 It requires the project config file to be run before.
 
 Usage:  
 python -m nkululeko.demo [--config CONFIG] [--file FILE] [--list LIST] [--folder FOLDER] [--outfile OUTFILE]  
 
 Options:   \n
 --config CONFIG     The base configuration file (default: exp.ini) \n  
@@ -16,25 +17,23 @@
 --folder FOLDER     A name of a folder where the files within the list are in   (default: ./) \n   
 --outfile OUTFILE   A filename to store the results in CSV  (default: None)  
 """
 import argparse
 import configparser
 import os
 
-import nkululeko.glob_conf as glob_conf
 from nkululeko.constants import VERSION
 from nkululeko.experiment import Experiment
+import nkululeko.glob_conf as glob_conf
 from nkululeko.utils.util import Util
 
 
 def main(src_dir):
-    parser = argparse.ArgumentParser(
-        description="Call the nkululeko DEMO framework.")
-    parser.add_argument("--config", default="exp.ini",
-                        help="The base configuration")
+    parser = argparse.ArgumentParser(description="Call the nkululeko DEMO framework.")
+    parser.add_argument("--config", default="exp.ini", help="The base configuration")
     parser.add_argument(
         "--file", help="A file that should be processed (16kHz mono wav)"
     )
     parser.add_argument(
         "--list",
         help=(
             "A file with a list of files, one per line, that should be"
```

### Comparing `nkululeko-0.83.3/nkululeko/demo_feats.py` & `nkululeko-0.84.0/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/demo_predictor.py` & `nkululeko-0.84.0/nkululeko/demo_predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # demo_predictor.py
 import os
 
-import audformat
-import audiofile
 import numpy as np
 import pandas as pd
 
+import audformat
+import audiofile
+
 import nkululeko.glob_conf as glob_conf
 from nkululeko.utils.util import Util
 
 
 class Demo_predictor:
     def __init__(self, model, file, is_list, feature_extractor, label_encoder, outfile):
-        """Constructor setting up name and configuration"""
+        """Constructor setting up name and configuration."""
         self.model = model
         self.feature_extractor = feature_extractor
         self.label_encoder = label_encoder
         self.is_list = is_list
         self.sr = 16000
         self.target = glob_conf.config["DATA"]["target"]
         self.util = Util("demo_predictor")
```

### Comparing `nkululeko-0.83.3/nkululeko/experiment.py` & `nkululeko-0.84.0/nkululeko/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # experiment.py: Main class for an experiment (nkululeko.nkululeko)
 import ast
 import os
 import pickle
 import random
 import time
 
-import audeer
-import audformat
 import numpy as np
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder
 
-import nkululeko.glob_conf as glob_conf
+import audeer
+import audformat
+
 from nkululeko.data.dataset import Dataset
 from nkululeko.data.dataset_csv import Dataset_CSV
 from nkululeko.demo_predictor import Demo_predictor
 from nkululeko.feat_extract.feats_analyser import FeatureAnalyser
 from nkululeko.feature_extractor import FeatureExtractor
 from nkululeko.file_checker import FileChecker
-from nkululeko.filter_data import DataFilter, filter_min_dur
+from nkululeko.filter_data import DataFilter
+from nkululeko.filter_data import filter_min_dur
+import nkululeko.glob_conf as glob_conf
 from nkululeko.plots import Plots
 from nkululeko.reporting.report import Report
 from nkululeko.runmanager import Runmanager
 from nkululeko.scaler import Scaler
 from nkululeko.test_predictor import TestPredictor
 from nkululeko.utils.util import Util
 
@@ -97,14 +99,15 @@
                 self.got_gender = True
             if data.got_age:
                 self.got_age = True
             if data.got_speaker:
                 self.got_speaker = True
             self.datasets.update({d: data})
         self.target = self.util.config_val("DATA", "target", "emotion")
+        glob_conf.set_target(self.target)
         # print target via debug
         self.util.debug(f"target: {self.target}")
         # print keys/column
         dbs = ",".join(list(self.datasets.keys()))
         labels = self.util.config_val("DATA", "labels", False)
         if labels:
             self.labels = ast.literal_eval(labels)
@@ -483,19 +486,15 @@
                 " should be [all | train | test]"
             )
         randomsplicer = Randomsplicer(df)
         df_ret = randomsplicer.run(sample_selection)
         return df_ret
 
     def analyse_features(self, needs_feats):
-        """
-        Do a feature exploration
-
-        """
-
+        """Do a feature exploration."""
         plot_feats = eval(
             self.util.config_val("EXPL", "feature_distributions", "False")
         )
         sample_selection = self.util.config_val("EXPL", "sample_selection", "all")
         # get the data labels
         if sample_selection == "all":
             df_labels = pd.concat([self.df_train, self.df_test])
@@ -507,15 +506,15 @@
             df_labels = self.df_test
             self.util.copy_flags(self.df_test, df_labels)
         else:
             self.util.error(
                 f"unknown sample selection specifier {sample_selection}, should"
                 " be [all | train | test]"
             )
-
+        self.util.debug(f"sampling selection: {sample_selection}")
         if self.util.config_val("EXPL", "value_counts", False):
             self.plot_distribution(df_labels)
 
         # check if data should be shown with the spotlight data visualizer
         spotlight = eval(self.util.config_val("EXPL", "spotlight", "False"))
         if spotlight:
             self.util.debug("opening spotlight tab in web browser")
@@ -533,17 +532,21 @@
         elif sample_selection == "test":
             df_feats = self.feats_test
         else:
             self.util.error(
                 f"unknown sample selection specifier {sample_selection}, should"
                 " be [all | train | test]"
             )
+        feat_analyser = FeatureAnalyser(sample_selection, df_labels, df_feats)
+        # check if SHAP features should be analysed
+        shap = eval(self.util.config_val("EXPL", "shap", "False"))
+        if shap:
+            feat_analyser.analyse_shap(self.runmgr.get_best_model())
 
         if plot_feats:
-            feat_analyser = FeatureAnalyser(sample_selection, df_labels, df_feats)
             feat_analyser.analyse()
 
         # check if a scatterplot should be done
         scatter_var = eval(self.util.config_val("EXPL", "scatter", "False"))
         scatter_target = self.util.config_val(
             "EXPL", "scatter.target", "['class_label']"
         )
@@ -688,15 +691,15 @@
         self.__dict__.update(tmp_dict)
         glob_conf.set_labels(self.labels)
 
     def save(self, filename):
         if self.runmgr.modelrunner.model.is_ann():
             self.runmgr.modelrunner.model = None
             self.util.warn(
-                "Save experiment: Can't pickle the learning model so saving without it."
+                "Save experiment: Can't pickle the trained model so saving without it. (it should be stored anyway)"
             )
         try:
             f = open(filename, "wb")
             pickle.dump(self.__dict__, f)
             f.close()
         except (TypeError, AttributeError) as error:
             self.feature_extractor.feat_extractor.model = None
```

### Comparing `nkululeko-0.83.3/nkululeko/explore.py` & `nkululeko-0.84.0/nkululeko/explore.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from nkululeko.constants import VERSION
 from nkululeko.experiment import Experiment
 from nkululeko.utils.util import Util
 
 
 def main(src_dir):
     parser = argparse.ArgumentParser(
-        description="Call the nkululeko EXPLORE framework.")
-    parser.add_argument("--config", default="exp.ini",
-                        help="The base configuration")
+        description="Call the nkululeko EXPLORE framework."
+    )
+    parser.add_argument("--config", default="exp.ini", help="The base configuration")
     args = parser.parse_args()
     if args.config is not None:
         config_file = args.config
     else:
         config_file = f"{src_dir}/exp.ini"
 
     # test if the configuration file exists
@@ -39,36 +39,42 @@
         f" {VERSION}"
     )
 
     if util.config_val("EXP", "no_warnings", False):
         import warnings
 
         warnings.filterwarnings("ignore")
-
-    # load the data
-    expr.load_datasets()
-
-    # split into train and test
-    expr.fill_train_and_tests()
-    util.debug(
-        f"train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}")
-
-    plot_feats = eval(util.config_val(
-        "EXPL", "feature_distributions", "False"))
-    tsne = eval(util.config_val("EXPL", "tsne", "False"))
-    scatter = eval(util.config_val("EXPL", "scatter", "False"))
-    spotlight = eval(util.config_val("EXPL", "spotlight", "False"))
-    model_type = util.config_val("EXPL", "model", False)
-    plot_tree = eval(util.config_val("EXPL", "plot_tree", "False"))
     needs_feats = False
-    if plot_feats or tsne or scatter or model_type or plot_tree:
-        # these investigations need features to explore
-        expr.extract_feats()
+    try:
+        # load the experiment
+        expr.load(f"{util.get_save_name()}")
         needs_feats = True
-    # explore
+    except FileNotFoundError:
+        # first time: load the data
+        expr.load_datasets()
+
+        # split into train and test
+        expr.fill_train_and_tests()
+        util.debug(
+            f"train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}"
+        )
+
+        plot_feats = eval(util.config_val("EXPL", "feature_distributions", "False"))
+        tsne = eval(util.config_val("EXPL", "tsne", "False"))
+        scatter = eval(util.config_val("EXPL", "scatter", "False"))
+        spotlight = eval(util.config_val("EXPL", "spotlight", "False"))
+        shap = eval(util.config_val("EXPL", "shap", "False"))
+        model_type = util.config_val("EXPL", "model", False)
+        plot_tree = eval(util.config_val("EXPL", "plot_tree", "False"))
+        needs_feats = False
+        if plot_feats or tsne or scatter or model_type or plot_tree or shap:
+            # these investigations need features to explore
+            expr.extract_feats()
+            needs_feats = True
+        # explore
     expr.analyse_features(needs_feats)
     expr.store_report()
     print("DONE")
 
 
 if __name__ == "__main__":
     cwd = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `nkululeko-0.83.3/nkululeko/export.py` & `nkululeko-0.84.0/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_analyser.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,47 @@
                 random_state=0,
             )
             importance = r["importances_mean"]
         else:
             importance = model.feature_importances_
         return importance
 
+    def analyse_shap(self, model):
+        """Shap analysis.
+
+        Use the best model from a previous run and analyse feature importance with SHAP.
+        https://m.mage.ai/how-to-interpret-and-explain-your-machine-learning-models-using-shap-values-471c2635b78e.
+        """
+        import shap
+
+        name = "my_shap_values"
+        if not self.util.exist_pickle(name):
+
+            explainer = shap.Explainer(
+                model.predict_shap,
+                self.features,
+                output_names=glob_conf.labels,
+                algorithm="permutation",
+                npermutations=5,
+            )
+            self.util.debug("computing SHAP values...")
+            shap_values = explainer(self.features)
+            self.util.to_pickle(shap_values, name)
+        else:
+            shap_values = self.util.from_pickle(name)
+        plt.tight_layout()
+        shap.plots.bar(shap_values)
+        fig_dir = self.util.get_path("fig_dir") + "../"  # one up because of the runs
+        exp_name = self.util.get_exp_name(only_data=True)
+        format = self.util.config_val("PLOT", "format", "png")
+        filename = f"_SHAP_{model.name}"
+        filename = f"{fig_dir}{exp_name}{filename}.{format}"
+        plt.savefig(filename)
+        self.util.debug(f"plotted SHAP feature importance tp {filename}")
+
     def analyse(self):
         models = ast.literal_eval(self.util.config_val("EXPL", "model", "['log_reg']"))
         model_name = "_".join(models)
         max_feat_num = int(self.util.config_val("EXPL", "max_feats", "10"))
         # https://scikit-learn.org/stable/modules/permutation_importance.html
         permutation = eval(self.util.config_val("EXPL", "permutation", "False"))
         importance = None
```

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_auddim.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_auddim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feats_whisper.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feats_whisper.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/featureset.py` & `nkululeko-0.84.0/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.84.0/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/feature_extractor.py` & `nkululeko-0.84.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/file_checker.py` & `nkululeko-0.84.0/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/filter_data.py` & `nkululeko-0.84.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/losses/loss_ccc.py` & `nkululeko-0.84.0/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.84.0/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/modelrunner.py` & `nkululeko-0.84.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/models/model.py` & `nkululeko-0.84.0/nkululeko/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 class Model:
     """Generic model class for linear (non-neural) algorithms."""
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         """Constructor taking the configuration and all dataframes."""
+        self.name = "undefined"
         self.df_train, self.df_test, self.feats_train, self.feats_test = (
             df_train,
             df_test,
             feats_train,
             feats_test,
         )
         self.model_type = "classic"
```

### Comparing `nkululeko-0.83.3/nkululeko/models/model_cnn.py` & `nkululeko-0.84.0/nkululeko/models/model_cnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
     is_classifier = True
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         """Constructor taking the configuration and all dataframes"""
         super().__init__(df_train, df_test, feats_train, feats_test)
         super().set_model_type("ann")
-        self.target = glob_conf.config["DATA"]["target"]
+        self.name = "cnn"
+        self.target = glob_conf.target
         labels = glob_conf.labels
         self.class_num = len(labels)
         # set up loss criterion
         criterion = self.util.config_val("MODEL", "loss", "cross")
         if criterion == "cross":
             self.criterion = torch.nn.CrossEntropyLoss()
         elif criterion == "f1":
@@ -82,16 +83,15 @@
                 transforms.ToTensor()
                 # transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))
             ]
         )
         train_set = self.Dataset_image(
             feats_train, df_train, self.target, transformations
         )
-        test_set = self.Dataset_image(
-            feats_test, df_test, self.target, transformations)
+        test_set = self.Dataset_image(feats_test, df_test, self.target, transformations)
         # Define data loaders
         self.trainloader = torch.utils.data.DataLoader(
             train_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
@@ -136,16 +136,15 @@
         self.set_testdata(df_test, feats_test)
 
     def train(self):
         self.model.train()
         losses = []
         for images, labels in self.trainloader:
             logits = self.model(images.to(self.device))
-            loss = self.criterion(logits, labels.to(
-                self.device, dtype=torch.int64))
+            loss = self.criterion(logits, labels.to(self.device, dtype=torch.int64))
             losses.append(loss.item())
             self.optimizer.zero_grad()
             loss.backward()
             self.optimizer.step()
         self.loss = (np.asarray(losses)).mean()
 
     def evaluate_model(self, model, loader, device):
@@ -165,24 +164,22 @@
                     logits[start_index:end_index, :],
                     labels.to(self.device, dtype=torch.int64),
                 )
                 losses.append(loss.item())
 
         self.loss_eval = (np.asarray(losses)).mean()
         predictions = logits.argmax(dim=1)
-        uar = recall_score(
-            targets.numpy(), predictions.numpy(), average="macro")
+        uar = recall_score(targets.numpy(), predictions.numpy(), average="macro")
         return uar, targets, predictions
 
     def predict(self):
         _, truths, predictions = self.evaluate_model(
             self.model, self.testloader, self.device
         )
-        uar, _, _ = self.evaluate_model(
-            self.model, self.trainloader, self.device)
+        uar, _, _ = self.evaluate_model(self.model, self.trainloader, self.device)
         report = Reporter(truths, predictions, self.run, self.epoch)
         try:
             report.result.loss = self.loss
         except AttributeError:  # if the model was loaded from disk the loss is unknown
             pass
         try:
             report.result.loss_eval = self.loss_eval
```

### Comparing `nkululeko-0.83.3/nkululeko/models/model_gmm.py` & `nkululeko-0.84.0/nkululeko/models/model_gmm.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 class GMM_model(Model):
     """An GMM model"""
 
     is_classifier = True
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         super().__init__(df_train, df_test, feats_train, feats_test)
+        self.name = "gmm"
         n_components = int(self.util.config_val("MODEL", "GMM_components", "4"))
-        covariance_type = self.util.config_val(
-            "MODEL", "GMM_covariance_type", "full"
-        )
+        covariance_type = self.util.config_val("MODEL", "GMM_covariance_type", "full")
         self.clf = mixture.GaussianMixture(
             n_components=n_components, covariance_type=covariance_type
         )
         # set up the classifier
```

### Comparing `nkululeko-0.83.3/nkululeko/models/model_knn.py` & `nkululeko-0.84.0/nkululeko/models/model_knn.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,12 +7,13 @@
 class KNN_model(Model):
     """An KNN model"""
 
     is_classifier = True
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         super().__init__(df_train, df_test, feats_train, feats_test)
+        self.name = "knn"
         method = self.util.config_val("MODEL", "KNN_weights", "uniform")
         k = int(self.util.config_val("MODEL", "K_val", "5"))
         self.clf = KNeighborsClassifier(
             n_neighbors=k, weights=method
         )  # set up the classifier
```

### Comparing `nkululeko-0.83.3/nkululeko/models/model_knn_reg.py` & `nkululeko-0.84.0/nkululeko/models/model_knn_reg.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,12 +7,13 @@
 class KNN_reg_model(Model):
     """An KNN model"""
 
     is_classifier = False
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         super().__init__(df_train, df_test, feats_train, feats_test)
+        self.name = "knn_reg"
         method = self.util.config_val("MODEL", "KNN_weights", "uniform")
         k = int(self.util.config_val("MODEL", "K_val", "5"))
         self.clf = KNeighborsRegressor(
             n_neighbors=k, weights=method
         )  # set up the classifier
```

### Comparing `nkululeko-0.83.3/nkululeko/models/model_mlp.py` & `nkululeko-0.84.0/nkululeko/models/model_mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # model_mlp.py
+import pandas as pd
+
 from nkululeko.utils.util import Util
 import nkululeko.glob_conf as glob_conf
 from nkululeko.models.model import Model
 from nkululeko.reporting.reporter import Reporter
 import torch
 import ast
 import numpy as np
@@ -16,14 +18,15 @@
 
     is_classifier = True
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         """Constructor taking the configuration and all dataframes"""
         super().__init__(df_train, df_test, feats_train, feats_test)
         super().set_model_type("ann")
+        self.name = "mlp"
         self.target = glob_conf.config["DATA"]["target"]
         labels = glob_conf.labels
         self.class_num = len(labels)
         # set up loss criterion
         criterion = self.util.config_val("MODEL", "loss", "cross")
         if criterion == "cross":
             self.criterion = torch.nn.CrossEntropyLoss()
@@ -83,16 +86,15 @@
         self.testloader = self.get_loader(feats_test, df_test, False)
 
     def train(self):
         self.model.train()
         losses = []
         for features, labels in self.trainloader:
             logits = self.model(features.to(self.device))
-            loss = self.criterion(logits, labels.to(
-                self.device, dtype=torch.int64))
+            loss = self.criterion(logits, labels.to(self.device, dtype=torch.int64))
             losses.append(loss.item())
             self.optimizer.zero_grad()
             loss.backward()
             self.optimizer.step()
         self.loss = (np.asarray(losses)).mean()
 
     def evaluate_model(self, model, loader, device):
@@ -112,24 +114,22 @@
                     logits[start_index:end_index, :].to(device),
                     labels.to(device, dtype=torch.int64),
                 )
                 losses.append(loss.item())
 
         self.loss_eval = (np.asarray(losses)).mean()
         predictions = logits.argmax(dim=1)
-        uar = recall_score(
-            targets.numpy(), predictions.numpy(), average="macro")
+        uar = recall_score(targets.numpy(), predictions.numpy(), average="macro")
         return uar, targets, predictions
 
     def predict(self):
         _, truths, predictions = self.evaluate_model(
             self.model, self.testloader, self.device
         )
-        uar, _, _ = self.evaluate_model(
-            self.model, self.trainloader, self.device)
+        uar, _, _ = self.evaluate_model(self.model, self.trainloader, self.device)
         report = Reporter(truths, predictions, self.run, self.epoch)
         try:
             report.result.loss = self.loss
         except AttributeError:  # if the model was loaded from disk the loss is unknown
             pass
         try:
             report.result.loss_eval = self.loss_eval
@@ -172,16 +172,26 @@
             self.linear = torch.nn.Sequential(layers)
 
         def forward(self, x):
             # x: (batch_size, channels, samples)
             x = x.squeeze(dim=1).float()
             return self.linear(x)
 
+    def predict_shap(self, features):
+        # predict outputs for all samples in SHAP format (pd. dataframe)
+        results = []
+        for index, row in features.iterrows():
+            feats = row.values
+            res_dict = self.predict_sample(feats)
+            class_key = max(res_dict, key=res_dict.get)
+            results.append(class_key)
+        return results
+
     def predict_sample(self, features):
-        """Predict one sample"""
+        """Predict one sample."""
         with torch.no_grad():
             features = torch.from_numpy(features)
             features = np.reshape(features, (-1, 1)).T
             logits = self.model(features.to(self.device))
             # logits = self.model(features)
         # if tensor conver to cpu
         if isinstance(logits, torch.Tensor):
```

### Comparing `nkululeko-0.83.3/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.84.0/nkululeko/models/model_mlp_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """MLP = multi layer perceptron"""
 
     is_classifier = False
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         """Constructor taking the configuration and all dataframes"""
         super().__init__(df_train, df_test, feats_train, feats_test)
+        self.name = "mlp_reg"
         super().set_model_type("ann")
         self.target = glob_conf.config["DATA"]["target"]
         labels = glob_conf.labels
         self.class_num = len(labels)
         # set up loss criterion
         criterion = self.util.config_val("MODEL", "loss", "mse")
         if criterion == "mse":
@@ -48,16 +49,15 @@
         try:
             layers = ast.literal_eval(layers_string)
         except KeyError as ke:
             self.util.error(f"Please provide MODEL layers: {ke}")
         drop = self.util.config_val("MODEL", "drop", False)
         if drop:
             self.util.debug(f"training with dropout: {drop}")
-        self.model = self.MLP(
-            feats_train.shape[1], layers, 1, drop).to(self.device)
+        self.model = self.MLP(feats_train.shape[1], layers, 1, drop).to(self.device)
         self.learning_rate = float(
             self.util.config_val("MODEL", "learning_rate", 0.0001)
         )
         # set up regularization
         self.optimizer = torch.optim.Adam(
             self.model.parameters(), lr=self.learning_rate
         )
@@ -92,18 +92,16 @@
         )
         return loss
 
     def predict(self):
         _, truths, predictions = self.evaluate_model(
             self.model, self.testloader, self.device
         )
-        result, _, _ = self.evaluate_model(
-            self.model, self.trainloader, self.device)
-        report = Reporter(truths.numpy(), predictions.numpy(),
-                          self.run, self.epoch)
+        result, _, _ = self.evaluate_model(self.model, self.trainloader, self.device)
+        report = Reporter(truths.numpy(), predictions.numpy(), self.run, self.epoch)
         try:
             report.result.loss = self.loss
         except AttributeError:  # if the model was loaded from disk the loss is unknown
             pass
         try:
             report.result.loss_eval = self.loss_eval
         except AttributeError:  # if the model was loaded from disk the loss is unknown
@@ -129,19 +127,17 @@
             self.label = label
 
         def __len__(self):
             return len(self.df)
 
         def __getitem__(self, item):
             index = self.df.index[item]
-            features = self.df_features.loc[index, :].values.astype(
-                "float32").squeeze()
+            features = self.df_features.loc[index, :].values.astype("float32").squeeze()
             labels = (
-                np.array([self.df.loc[index, self.label]]
-                         ).astype("float32").squeeze()
+                np.array([self.df.loc[index, self.label]]).astype("float32").squeeze()
             )
             return features, labels
 
     class MLP(torch.nn.Module):
         def __init__(self, i, layers, o, drop):
             super().__init__()
             sorted_layers = sorted(layers.items(), key=lambda x: x[1])
@@ -190,16 +186,15 @@
         losses = []
         with torch.no_grad():
             for index, (features, labels) in enumerate(loader):
                 start_index = index * loader.batch_size
                 end_index = (index + 1) * loader.batch_size
                 if end_index > len(loader.dataset):
                     end_index = len(loader.dataset)
-                logits[start_index:end_index] = model(
-                    features.to(device)).reshape(-1)
+                logits[start_index:end_index] = model(features.to(device)).reshape(-1)
                 targets[start_index:end_index] = labels
                 loss = self.criterion(
                     logits[start_index:end_index].to(
                         device,
                     ),
                     labels.to(device),
                 )
```

### Comparing `nkululeko-0.83.3/nkululeko/models/model_svm.py` & `nkululeko-0.84.0/nkululeko/models/model_svm.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class SVM_model(Model):
     """An SVM model"""
 
     is_classifier = True
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         super().__init__(df_train, df_test, feats_train, feats_test)
+        self.name = "svm"
         c = float(self.util.config_val("MODEL", "C_val", "0.001"))
         if eval(self.util.config_val("MODEL", "class_weight", "False")):
             class_weight = "balanced"
         else:
             class_weight = None
         kernel = self.util.config_val("MODEL", "kernel", "rbf")
         self.clf = svm.SVC(
```

### Comparing `nkululeko-0.83.3/nkululeko/models/model_svr.py` & `nkululeko-0.84.0/nkululeko/models/model_svr.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class SVR_model(Model):
     """An SVR model"""
 
     is_classifier = False
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         super().__init__(df_train, df_test, feats_train, feats_test)
+        self.name = "svr"
         c = float(self.util.config_val("MODEL", "C_val", "0.001"))
         #  kernel{‘linear’, ‘poly’, ‘rbf’, ‘sigmoid’, ‘precomputed’} or callable, default=’rbf’
         kernel = self.util.config_val("MODEL", "kernel", "rbf")
         self.clf = svm.SVR(kernel=kernel, C=c)  # set up the classifier
 
     def set_C(self, c):
         """Set the C parameter"""
```

### Comparing `nkululeko-0.83.3/nkululeko/multidb.py` & `nkululeko-0.84.0/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/nkuluflag.py` & `nkululeko-0.84.0/nkululeko/nkuluflag.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/nkululeko.py` & `nkululeko-0.84.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/plots.py` & `nkululeko-0.84.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/predict.py` & `nkululeko-0.84.0/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/reporting/defines.py` & `nkululeko-0.84.0/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/reporting/latex_writer.py` & `nkululeko-0.84.0/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/reporting/report.py` & `nkululeko-0.84.0/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/reporting/report_item.py` & `nkululeko-0.84.0/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/reporting/reporter.py` & `nkululeko-0.84.0/nkululeko/reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/reporting/result.py` & `nkululeko-0.84.0/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/resample.py` & `nkululeko-0.84.0/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/runmanager.py` & `nkululeko-0.84.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/scaler.py` & `nkululeko-0.84.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/segment.py` & `nkululeko-0.84.0/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.84.0/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.84.0/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/syllable_nuclei.py` & `nkululeko-0.84.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/test.py` & `nkululeko-0.84.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/test_predictor.py` & `nkululeko-0.84.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/utils/files.py` & `nkululeko-0.84.0/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/utils/stats.py` & `nkululeko-0.84.0/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/nkululeko/utils/util.py` & `nkululeko-0.84.0/nkululeko/utils/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # util.py
-import pandas as pd
 import ast
+import configparser
+import os.path
+import pickle
 import sys
+
 import numpy as np
-import os.path
-import configparser
+import pandas as pd
+
 import audeer
 import audformat
 
 
 class Util:
     # a list of words that need not to be warned upon if default values are used
     stopvals = [
@@ -291,14 +294,36 @@
         with open(file_name, "w") as text_file:
             text_file.write(all)
             text_file.write(
                 f"\nmean: {vals.mean():.3f}, max: {vals.max():.3f}, max_index:"
                 f" {vals.argmax()}"
             )
 
+    def exist_pickle(self, name):
+        store = self.get_path("store")
+        name = "/".join([store, name]) + ".pkl"
+        if os.path.isfile(name):
+            return True
+        return False
+
+    def to_pickle(self, anyobject, name):
+        store = self.get_path("store")
+        name = "/".join([store, name]) + ".pkl"
+        self.debug(f"saving {name}")
+        with open(name, "wb") as handle:
+            pickle.dump(anyobject, handle)
+
+    def from_pickle(self, name):
+        store = self.get_path("store")
+        name = "/".join([store, name]) + ".pkl"
+        self.debug(f"loading {name}")
+        with open(name, "rb") as handle:
+            any_opject = pickle.load(handle)
+        return any_opject
+
     def write_store(self, df, storage, format):
         if format == "pkl":
             df.to_pickle(storage)
         elif format == "csv":
             df.to_csv(storage)
         else:
             self.error(f"unkown store format: {format}")
```

### Comparing `nkululeko-0.83.3/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.84.0/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.83.3
+Version: 0.84.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,19 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.84.0
+--------------
+* added SHAP analysis
+* started with finetuning
+
 Version 0.83.3
 --------------
 * fixed a naming error in trill features that prevented storage of experiment
 
 Version 0.83.2
 --------------
 * added default cuda if present and not stated
```

### Comparing `nkululeko-0.83.3/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.84.0/nkululeko.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 nkululeko/resample.py
 nkululeko/runmanager.py
 nkululeko/scaler.py
 nkululeko/segment.py
 nkululeko/syllable_nuclei.py
 nkululeko/test.py
 nkululeko/test_predictor.py
+nkululeko/test_pretrain.py
 nkululeko.egg-info/PKG-INFO
 nkululeko.egg-info/SOURCES.txt
 nkululeko.egg-info/dependency_links.txt
 nkululeko.egg-info/requires.txt
 nkululeko.egg-info/top_level.txt
 nkululeko/augmenting/__init__.py
 nkululeko/augmenting/augmenter.py
```

### Comparing `nkululeko-0.83.3/setup.cfg` & `nkululeko-0.84.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.3/venv/bin/activate_this.py` & `nkululeko-0.84.0/venv/bin/activate_this.py`

 * *Files identical despite different names*

