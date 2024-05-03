# Comparing `tmp/ligo-followup-advocate-1.2.8.tar.gz` & `tmp/ligo_followup_advocate-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-followup-advocate-1.2.8.tar", last modified: Tue Oct 31 18:31:10 2023, max compression
+gzip compressed data, was "ligo_followup_advocate-1.2.9.tar", last modified: Fri May  3 20:11:57 2024, max compression
```

## Comparing `ligo-followup-advocate-1.2.8.tar` & `ligo_followup_advocate-1.2.9.tar`

### file list

```diff
@@ -1,168 +1,181 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.465580 ligo-followup-advocate-1.2.8/
--rw-rw-rw-   0 root         (0) root         (0)    17895 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/COPYING.md
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1063 2023-10-31 18:31:10.465580 ligo-followup-advocate-1.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.435580 ligo-followup-advocate-1.2.8/ligo/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.436580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/
--rw-rw-rw-   0 root         (0) root         (0)    28200 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-10-31 18:31:10.466580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/jinja.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.438580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2972 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/RAVEN_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/RAVEN_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/authors.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/compare_skymaps.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1048 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/em_bright.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2626 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/initial_body.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/initial_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/llama_alert_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/llama_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2483 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/llama_track_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)    10525 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1694 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/p_astro.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/retraction.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/skymap_info.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/update_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/userguide_conclusion.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.438580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.434580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.439580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.439580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.439580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1133/
--rw-rw-rw-   0 root         (0) root         (0)     1877 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1133/event.json
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1133/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.439580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1134/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1134/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.440580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1134/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1134/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.440580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.440580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.441580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.441580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.441580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.442580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.442580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E5678/
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E5678/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.442580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E5678/files/
--rw-rw-rw-   0 root         (0) root         (0)     5761 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E5678/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.442580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1122/
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1122/event.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.443580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1234/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1234/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.443580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1235/
--rw-rw-rw-   0 root         (0) root         (0)     3982 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1235/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.443580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2468/
--rw-rw-rw-   0 root         (0) root         (0)     3956 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2468/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.443580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2468/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2468/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2468/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.443580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2469/
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2469/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.443580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2469/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2469/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2469/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.444580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5566/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5566/event.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5566/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.444580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5678/
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5678/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.444580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5679/
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5679/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5679/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.445580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.449580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/
--rw-rw-rw-   0 root         (0) root         (0)     6797 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
--rw-rw-rw-   0 root         (0) root         (0)     6795 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)     1832 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7997 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5897 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.450580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.451580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/files/
--rw-rw-rw-   0 root         (0) root         (0)     4476 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)     4047 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/files.json
--rw-rw-rw-   0 root         (0) root         (0)     4911 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.452580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.464580 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/RapidPE_RIFT.p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/RapidPE_RIFT.p_astro.json,0
--rw-rw-rw-   0 root         (0) root         (0)     8946 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)     8933 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files.json
--rw-rw-rw-   0 root         (0) root         (0)     8228 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5616 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/voevents.json
--rw-rw-rw-   0 root         (0) root         (0)     7555 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3113 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/ligo/followup_advocate/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 18:31:10.465580 ligo-followup-advocate-1.2.8/ligo_followup_advocate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-10-31 18:31:10.000000 ligo-followup-advocate-1.2.8/ligo_followup_advocate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7128 2023-10-31 18:31:10.000000 ligo-followup-advocate-1.2.8/ligo_followup_advocate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-31 18:31:10.000000 ligo-followup-advocate-1.2.8/ligo_followup_advocate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-10-31 18:31:10.000000 ligo-followup-advocate-1.2.8/ligo_followup_advocate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-10-31 18:31:10.000000 ligo-followup-advocate-1.2.8/ligo_followup_advocate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-10-31 18:31:10.000000 ligo-followup-advocate-1.2.8/ligo_followup_advocate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-10-31 18:31:10.466580 ligo-followup-advocate-1.2.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      496 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    86677 2023-10-31 18:30:58.000000 ligo-followup-advocate-1.2.8/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.930163 ligo_followup_advocate-1.2.9/
+-rw-rw-rw-   0 root         (0) root         (0)    17895 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/COPYING.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-03 20:11:57.930163 ligo_followup_advocate-1.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.893162 ligo_followup_advocate-1.2.9/ligo/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.894162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/
+-rw-rw-rw-   0 root         (0) root         (0)    28291 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-03 20:11:57.931163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/jinja.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.897162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/RAVEN_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      944 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/RAVEN_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/authors.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      699 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/combine_skymaps.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/compare_skymaps.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/em_bright.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2644 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/initial_body.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      437 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/initial_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/llama_alert_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/llama_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2483 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/llama_track_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)    10761 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      344 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      626 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/p_astro.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/retraction.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/skymap_info.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/update_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/userguide_conclusion.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.898162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.892162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.898162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.899162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.899162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1133/
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1133/event.json
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1133/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.899162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1134/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1134/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.899162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1134/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1134/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.900162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.900162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.901162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.901162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.902162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.902162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      991 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.903162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E5678/
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E5678/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.903162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)     5761 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E5678/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.903162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1122/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.903162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1123/
+-rw-rw-rw-   0 root         (0) root         (0)     1933 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1123/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1123/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.904163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1234/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1234/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.904163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1235/
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1235/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.904163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2468/
+-rw-rw-rw-   0 root         (0) root         (0)     3956 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2468/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.904163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2468/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2468/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.905162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2469/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2469/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.905162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2469/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2469/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2469/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.905162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5566/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5566/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5566/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.905162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5678/
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5678/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.906162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5679/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5679/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5679/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.906162 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.911163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)     6797 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6795 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7997 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5897 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.912163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.913163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  1065600 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.914163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2469/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.915163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2469/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2469/files/S2468-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  1065600 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2469/files/cwb.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2469/files/significance_subthreshold_lvc-i3.json
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2469/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2469/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     3394 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2469/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2469/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.916163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.929163 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/RapidPE_RIFT.p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/RapidPE_RIFT.p_astro.json,0
+-rw-rw-rw-   0 root         (0) root         (0)     8946 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)     8933 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     8228 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/voevents.json
+-rw-rw-rw-   0 root         (0) root         (0)     7802 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3113 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/ligo/followup_advocate/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:11:57.930163 ligo_followup_advocate-1.2.9/ligo_followup_advocate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-03 20:11:57.000000 ligo_followup_advocate-1.2.9/ligo_followup_advocate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7704 2024-05-03 20:11:57.000000 ligo_followup_advocate-1.2.9/ligo_followup_advocate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 20:11:57.000000 ligo_followup_advocate-1.2.9/ligo_followup_advocate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-03 20:11:57.000000 ligo_followup_advocate-1.2.9/ligo_followup_advocate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-03 20:11:57.000000 ligo_followup_advocate-1.2.9/ligo_followup_advocate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-03 20:11:57.000000 ligo_followup_advocate-1.2.9/ligo_followup_advocate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2024-05-03 20:11:57.931163 ligo_followup_advocate-1.2.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      496 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-03 20:11:48.000000 ligo_followup_advocate-1.2.9/versioneer.py
```

### Comparing `ligo-followup-advocate-1.2.8/COPYING.md` & `ligo_followup_advocate-1.2.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/PKG-INFO` & `ligo_followup_advocate-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.8
+Version: 1.2.9
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.8/README.md` & `ligo_followup_advocate-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/__init__.py` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,18 @@
         client = rest.GraceDb(service)
 
     kwargs = dict()
     kwargs = _update_raven_parameters(gracedb_id, kwargs, client)
     kwargs.update(main_dict(gracedb_id, client=client))
     kwargs.update(update_alert=False)
     kwargs.update(text_width=text_width(remove_text_wrap))
+    # Add RAVEN citation
+    citation_index = kwargs['citation_index']
+    citation_index['raven'] = max(citation_index.values()) + 1
+    kwargs['citation_index'] = citation_index
 
     subject = (
         env.get_template('RAVEN_subject.jinja2').render(**kwargs)
         .strip())
     body = (
         env.get_template('RAVEN_circular.jinja2').render(**kwargs)
         .strip())
@@ -429,32 +433,34 @@
     if isinstance(update_types, str):
         update_types = update_types.split(',')
 
     # Adjust files for update type alert
     citation_index = {}
     skymaps = []
     index = 1
-    if 'em_bright' in update_types or 'sky_localization' in update_types or \
-            'p_astro' in update_types:
-        updated_skymap = kwargs.get('skymaps')[-1]
-        kwargs.update(updated_skymap=updated_skymap)
-        skymaps = [updated_skymap]
-        if 'sky_localization' in update_types:
+
+    updated_skymap = kwargs.get('skymaps')[-1]
+    kwargs.update(updated_skymap=updated_skymap)
+    skymaps = [updated_skymap]
+    if 'sky_localization' in update_types:
+        citation_index[updated_skymap['pipeline'].lower()] = index
+        index += 1
+    if 'p_astro' in update_types and \
+            kwargs.get('p_astro_pipeline') == 'rapidpe_rift':
+        citation_index['rapidpe_rift'] = index
+        index += 1
+    if 'em_bright' in update_types:
+        # If not already cited, cite sky map pipeline for em_bright
+        if updated_skymap['pipeline'].lower() not in citation_index.keys():
             citation_index[updated_skymap['pipeline'].lower()] = index
             index += 1
-        if 'p_astro' in update_types and \
-                kwargs.get('p_astro_pipeline') == 'rapidpe_rift':
-            citation_index['rapidpe_rift'] = index
-            index += 1
-        if 'em_bright' in update_types:
-            # If not already cited, cite sky map pipeline for em_bright
-            if updated_skymap['pipeline'].lower() not in citation_index.keys():
-                citation_index[updated_skymap['pipeline'].lower()] = index
-                index += 1
-            citation_index['em_bright'] = index
+        citation_index['em_bright'] = index
+        index += 1
+    if 'raven' in update_types:
+        citation_index['raven'] = index
 
     kwargs.update(skymaps=skymaps,
                   citation_index=citation_index,
                   all_pipelines=[],
                   update_alert=True)
 
     if 'raven' in update_types:
```

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/jinja.py` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/jinja.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/RAVEN_circular.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/RAVEN_circular.jinja2`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 {% from 'macros.jinja2' import naturalfar, grbmission, grbmission_targeted, naturalotherexternalpipelines, propername %}
 {% if not update_alert %}{% include 'authors.jinja2' %}
 
 {% include 'initial_body.jinja2' %}
 {% endif %}
 {% filter rewrap(text_width) %}
-A search performed by the RAVEN pipeline found a temporal coincidence between
+A search performed by the RAVEN pipeline [{{citation_index['raven']}}] found a temporal coincidence between
 {{gracedb_id}} and a {% if snews %}SNEWS supernova{% elif grb %}{% if subthreshold %}sub-threshold {% endif %}{{grbmission(external_pipeline)}}{% endif %} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.nasa.gov/circulars, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
 The {% if snews %}neutrino{% elif grb %}GRB{% endif %} trigger time is {{latency}} seconds {{beforeafter}} the GW candidate event.
 {% if grb %}
 The estimated joint false alarm rate for the coincidence using just timing info is {{naturalfar(time_coinc_far)}}.
 {% if subthreshold_targeted %}The GRB candidate was found during a joint targeted search between the LIGO/Virgo/KAGRA collaboration and {{grbmission_targeted(external_pipeline)}}, and has a false alarm rate of {{naturalfar(far_grb)}}. {% endif %}
 {% if other_ext_pipelines %}RAVEN has also identified {% if other_ext_pipelines|length == 1 %}an additional detection{% elif other_ext_pipelines|length > 1%}additional detections{% endif %} from {{naturalotherexternalpipelines(other_ext_pipelines)}}.{% endif %}
 {% endif %}
 
 {% if combined_skymap %}
-{% if combined_skymaps|length == 1 %}A combined sky map is{% else %}Combined sky maps are{% endif %} also available:
-{% for skymap in combined_skymaps %}
- * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% elif skymap.alert_type == 'earlywarning' %}early-warning{% else %}updated{% endif %} localization, distributed via GCN notice about {{skymap.latency|abs|naturaldelta}} {% if skymap.latency < 0 %}before {% else %}after {% endif %}the candidate event time.
-{% endfor %}
-
-For the {{combined_skymap}} sky map, the {{cl}}% credible region is {{combined_skymap_greedy_area|round|int}} deg2.
+{% include 'combine_skymaps.jinja2' %}
 {% endif %}
 {% if external_pipeline|lower == 'swift'%}
 The joint localization is dominated by the {{grbmission(external_pipeline)}} candidate, which was identified with right ascension, declination of {{'%0.3f' % ext_ra|float}}, {{'%0.3f' % ext_dec|float}}{% if ext_error %} and 90% containment error radius of {{'%0.3f' % ext_error|float}} deg{% endif %}.
 {% endif %}
 {% if combined_skymap and space_time_coinc_far is not none %}
 Considering the overlap of the individual sky maps, the estimated joint false alarm rate for the spatial and temporal coincidence is {{naturalfar(space_time_coinc_far)}}.
 {% elif combined_skymap and space_time_coinc_far is none %}
```

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/RAVEN_subject.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/RAVEN_subject.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/authors.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/authors.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/em_bright.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/em_bright.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/initial_body.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/initial_body.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% from 'macros.jinja2' import oxford_commas, evidence_for, probability,
                             naturalinstruments, naturalfar,
                             naturalclassifications, naturalpipelines,
                             naturalearlywarningpipelines,
                             renamegroup, citeskymap %}
 {% filter rewrap(text_width) %}
-We identified the {{renamegroup(group)}} candidate {{gracedb_id}} during real-time processing of data from
+We identified the {{renamegroup(group, pipeline, search)}} candidate {{gracedb_id}} during real-time processing of data from
 {{naturalinstruments(instruments, )}} at {{utctime}} UTC (GPS time: {{gpstime}}).
 The candidate was found by the {{naturalpipelines(all_pipelines, citation_index)}}
 analysis pipeline{% if all_pipelines|length > 1 %}s{% endif %}.
 {% if early_warning_alert and early_warning_pipelines %}
 An early-warning alert was issued for this candidate, detected by the {{naturalearlywarningpipelines(early_warning_pipelines, citation_index)}} early-warning pipeline{% if early_warning_pipelines|length > 1 %}s{% endif %}.
 {% endif %}
```

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/llama_alert_circular.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/llama_alert_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/llama_track_circular.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/llama_track_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/macros.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/macros.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -190,16 +190,16 @@
 {%- endif %} ({{probability(item[1])}})
 {%- endcall %}
 {%- endmacro %}
 
 
 Macro to replace jargon terms CBC and Burst.
 
-{%- macro renamegroup(group) -%}
-{%- if group|lower == 'cbc' -%}
+{%- macro renamegroup(group, pipeline, search) -%}
+{%- if group|lower == 'cbc' or (pipeline|lower == 'cwb' and search|lower == 'bbh') -%}
 compact binary merger
 {%- elif group|lower == 'burst' -%}
 unmodeled transient
 {%- else -%}
 {{group}}
 {%- endif -%}
 {%- endmacro -%}
@@ -260,8 +260,9 @@
                     'pygrb': 'Williamson et al. PRD 90, 122004 (2014) doi:10.1103/PhysRevD.90.122004',
                     'xpipeline': 'Was et al. PRD 86, 022003 (2012) doi:10.1103/PhysRevD.86.022003',
                     'llama': 'Baret et al., Astroparticle Physics 35, 1 (2011) doi:10.1016/j.astropartphys.2011.04.001',
                     'llama_stat': 'Bartos et al. PRD 100, 083017 (2019) doi:10.1103/PhysRevD.100.083017 and Countryman et al. (2019) arXiv:1901.05486',
                     'bayestar': 'Singer & Price PRD 93, 024013 (2016) doi:10.1103/PhysRevD.93.024013',
                     'bilby': 'Ashton et al. ApJS 241, 27 (2019) doi:10.3847/1538-4365/ab06fc and Morisaki et al. (2023) arXiv:2307.13380',
                     'lalinference': 'Veitch et al. PRD 91, 042003 (2015) doi:10.1103/PhysRevD.91.042003',
-                    'rapidpe_rift': 'Rose et al. (2022) arXiv:2201.05263 and Pankow et al. PRD 92, 023002 (2015) doi:10.1103/PhysRevD.92.023002'} %}
+                    'rapidpe_rift': 'Rose et al. (2022) arXiv:2201.05263 and Pankow et al. PRD 92, 023002 (2015) doi:10.1103/PhysRevD.92.023002',
+                    'raven': 'Urban, A. L. 2016, Ph.D. Thesis https://dc.uwm.edu/etd/1218 and Piotrzkowski, B. J. 2022, Ph.D. Thesis https://dc.uwm.edu/etd/3060'} %}
```

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/p_astro.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/p_astro.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/retraction.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/retraction.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/skymap_info.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/skymap_info.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/templates/update_circular.jinja2` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/templates/update_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1122/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1133/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1133/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1134/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1134/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1134/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1134/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/files/initial.data` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1234/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/files/initial.data` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E1235/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E2244/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E2244/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E5678/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/E5678/files/initial.data` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/E5678/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1122/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1122/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1234/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1234/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1235/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M1235/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2468/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2468/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2468/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2469/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2469/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M2469/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M2469/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5566/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5566/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5566/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5566/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5678/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5678/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5679/event.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5679/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/M5679/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/M5679/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/logs.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/superevent.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S1234/voevents.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S1234/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/logs.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/superevent.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S2468/voevents.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S2468/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/files.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/logs.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/superevent.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/data/S5678/voevents.json` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/data/S5678/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/test/test_tool.py` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/test/test_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,20 @@
 @pytest.mark.parametrize('wrap_text', [None, '--remove_text_wrap'])
 def test_burst_compose(mock_gracedb, wrap_text):
     main(remove_nones(['--service', 'https://gracedb.invalid/api/', wrap_text,
                        'compose', 'S2468']))
 
 
 @pytest.mark.parametrize('wrap_text', [None, '--remove_text_wrap'])
+def test_cwb_burst_compose(mock_gracedb, wrap_text):
+    main(remove_nones(['--service', 'https://gracedb.invalid/api/', wrap_text,
+                       'compose', 'S2469']))
+
+
+@pytest.mark.parametrize('wrap_text', [None, '--remove_text_wrap'])
 def test_skymap_update(mock_gracedb, wrap_text):
     main(remove_nones(['--service', 'https://gracedb.invalid/api/', wrap_text,
                        'compose_update', 'S5678', ['sky_localization']]))
 
 
 @pytest.mark.parametrize('wrap_text', [None, '--remove_text_wrap'])
 def test_raven_update(mock_gracedb, wrap_text):
```

### Comparing `ligo-followup-advocate-1.2.8/ligo/followup_advocate/tool.py` & `ligo_followup_advocate-1.2.9/ligo/followup_advocate/tool.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/ligo_followup_advocate.egg-info/PKG-INFO` & `ligo_followup_advocate-1.2.9/ligo_followup_advocate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.8
+Version: 1.2.9
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.8/ligo_followup_advocate.egg-info/SOURCES.txt` & `ligo_followup_advocate-1.2.9/ligo_followup_advocate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ligo/followup_advocate/_version.py
 ligo/followup_advocate/jinja.py
 ligo/followup_advocate/tool.py
 ligo/followup_advocate/templates/RAVEN_circular.jinja2
 ligo/followup_advocate/templates/RAVEN_subject.jinja2
 ligo/followup_advocate/templates/__init__.py
 ligo/followup_advocate/templates/authors.jinja2
+ligo/followup_advocate/templates/combine_skymaps.jinja2
 ligo/followup_advocate/templates/compare_skymaps.jinja2
 ligo/followup_advocate/templates/em_bright.jinja2
 ligo/followup_advocate/templates/initial_body.jinja2
 ligo/followup_advocate/templates/initial_circular.jinja2
 ligo/followup_advocate/templates/llama_alert_circular.jinja2
 ligo/followup_advocate/templates/llama_subject.jinja2
 ligo/followup_advocate/templates/llama_track_circular.jinja2
@@ -66,14 +67,16 @@
 ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
 ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
 ligo/followup_advocate/test/data/E5678/event.json
 ligo/followup_advocate/test/data/E5678/files.json
 ligo/followup_advocate/test/data/E5678/files/initial.data
 ligo/followup_advocate/test/data/M1122/event.json
 ligo/followup_advocate/test/data/M1122/files.json
+ligo/followup_advocate/test/data/M1123/event.json
+ligo/followup_advocate/test/data/M1123/files.json
 ligo/followup_advocate/test/data/M1234/event.json
 ligo/followup_advocate/test/data/M1234/files.json
 ligo/followup_advocate/test/data/M1235/event.json
 ligo/followup_advocate/test/data/M1235/files.json
 ligo/followup_advocate/test/data/M2468/event.json
 ligo/followup_advocate/test/data/M2468/files.json
 ligo/followup_advocate/test/data/M2468/files/p_astro.json
@@ -101,14 +104,21 @@
 ligo/followup_advocate/test/data/S2468/files.json
 ligo/followup_advocate/test/data/S2468/logs.json
 ligo/followup_advocate/test/data/S2468/superevent.json
 ligo/followup_advocate/test/data/S2468/voevents.json
 ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
 ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
 ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
+ligo/followup_advocate/test/data/S2469/files.json
+ligo/followup_advocate/test/data/S2469/logs.json
+ligo/followup_advocate/test/data/S2469/superevent.json
+ligo/followup_advocate/test/data/S2469/voevents.json
+ligo/followup_advocate/test/data/S2469/files/S2468-1-Initial.xml
+ligo/followup_advocate/test/data/S2469/files/cwb.multiorder.fits
+ligo/followup_advocate/test/data/S2469/files/significance_subthreshold_lvc-i3.json
 ligo/followup_advocate/test/data/S5678/files.json
 ligo/followup_advocate/test/data/S5678/logs.json
 ligo/followup_advocate/test/data/S5678/superevent.json
 ligo/followup_advocate/test/data/S5678/voevents.json
 ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
 ligo/followup_advocate/test/data/S5678/files/RapidPE_RIFT.p_astro.json
 ligo/followup_advocate/test/data/S5678/files/RapidPE_RIFT.p_astro.json,0
```

### Comparing `ligo-followup-advocate-1.2.8/setup.cfg` & `ligo_followup_advocate-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.8/versioneer.py` & `ligo_followup_advocate-1.2.9/versioneer.py`

 * *Files identical despite different names*

