# Comparing `tmp/hhd-2.6.5.tar.gz` & `tmp/hhd-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhd-2.6.5.tar", last modified: Thu May  2 19:52:42 2024, max compression
+gzip compressed data, was "hhd-2.7.0.tar", last modified: Fri May  3 12:17:24 2024, max compression
```

## Comparing `hhd-2.6.5.tar` & `hhd-2.7.0.tar`

### file list

```diff
@@ -1,147 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 19:52:31.000000 hhd-2.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 19:52:31.000000 hhd-2.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-05-02 19:52:42.631867 hhd-2.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-02 19:52:31.000000 hhd-2.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-05-02 19:52:31.000000 hhd-2.6.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:52:42.631867 hhd-2.6.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.615867 hhd-2.6.5/src/hhd/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/contrib/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37047 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/hide.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/ioctl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/lib/uhid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/physical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/evdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/hidraw.py
--rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/imu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/physical/rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/virtual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/virtual/dualsense/
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/dualsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/dualsense/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/virtual/sd/
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/sd/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.619867 hhd-2.6.5/src/hhd/controller/virtual/uinput/
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/uinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/controller/virtual/uinput/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/hhd/device/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/generic/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/generic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/generic/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/hhd/device/gpd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/gpd/win/
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/gpd/win/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/gpd/win/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/gpd/win/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/gpd/win/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/legion_go/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/gyro_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/legion_go/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/orange_pi/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/orange_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/orange_pi/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/orange_pi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/orange_pi/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/device/rog_ally/
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/device/rog_ally/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.623867 hhd-2.6.5/src/hhd/http/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/http/static/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/static/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/http/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/hhd/i18n/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-05-02 19:52:39.000000 hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo
--rw-r--r--   0 runner    (1001) docker     (127)    22062 2024-05-02 19:52:39.000000 hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/src/hhd/i18n/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-02 19:52:39.000000 hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-02 19:52:39.000000 hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.627867 hhd-2.6.5/src/hhd/plugins/display/
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/display/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/gyro.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/outputs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/src/hhd/plugins/overlay/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13232 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/overlay/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/src/hhd/plugins/powerbutton/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/powerbutton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/powerbutton/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/powerbutton/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/powerbutton/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/touchpad.yml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/sections.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-02 19:52:31.000000 hhd-2.6.5/src/hhd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/src/hhd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 19:52:42.000000 hhd-2.6.5/src/hhd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.611867 hhd-2.6.5/usr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.615867 hhd-2.6.5/usr/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/modules-load.d/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/modules-load.d/hhd-user.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.615867 hhd-2.6.5/usr/lib/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/systemd/system/hhd@.service
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/systemd/system/hhd_local@.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/systemd/user/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/systemd/user/hhd-user.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.615867 hhd-2.6.5/usr/lib/udev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/udev/hwdb.d/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/udev/hwdb.d/83-hhd.hwdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:52:42.631867 hhd-2.6.5/usr/lib/udev/rules.d/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/udev/rules.d/83-hhd-user.rules
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-02 19:52:31.000000 hhd-2.6.5/usr/lib/udev/rules.d/83-hhd.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.889871 hhd-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-03 12:17:15.000000 hhd-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-03 12:17:15.000000 hhd-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15418 2024-05-03 12:17:24.889871 hhd-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-03 12:17:15.000000 hhd-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-03 12:17:15.000000 hhd-2.7.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:17:24.889871 hhd-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.865872 hhd-2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.869871 hhd-2.7.0/src/hhd/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.873871 hhd-2.7.0/src/hhd/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/contrib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/contrib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/contrib/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/contrib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/contrib/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.873871 hhd-2.7.0/src/hhd/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37161 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.873871 hhd-2.7.0/src/hhd/controller/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/lib/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/lib/hide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/lib/ioctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/lib/uhid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.873871 hhd-2.7.0/src/hhd/controller/physical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/physical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/physical/evdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/physical/hidraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20715 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/physical/imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/physical/rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.873871 hhd-2.7.0/src/hhd/controller/virtual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/virtual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.873871 hhd-2.7.0/src/hhd/controller/virtual/dualsense/
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/virtual/dualsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/virtual/dualsense/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.877871 hhd-2.7.0/src/hhd/controller/virtual/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/virtual/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/virtual/sd/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.877871 hhd-2.7.0/src/hhd/controller/virtual/uinput/
+-rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/virtual/uinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/virtual/uinput/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/controller/virtual/uinput/monkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.865872 hhd-2.7.0/src/hhd/device/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.877871 hhd-2.7.0/src/hhd/device/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/generic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/generic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/generic/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.865872 hhd-2.7.0/src/hhd/device/gpd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.877871 hhd-2.7.0/src/hhd/device/gpd/win/
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/gpd/win/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/gpd/win/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/gpd/win/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/gpd/win/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.877871 hhd-2.7.0/src/hhd/device/legion_go/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/legion_go/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17329 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/legion_go/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/legion_go/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/legion_go/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/legion_go/gyro_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/legion_go/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.881872 hhd-2.7.0/src/hhd/device/orange_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/orange_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/orange_pi/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/orange_pi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/orange_pi/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.881872 hhd-2.7.0/src/hhd/device/rog_ally/
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/rog_ally/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/rog_ally/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/rog_ally/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/rog_ally/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/device/rog_ally/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.881872 hhd-2.7.0/src/hhd/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/http/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/http/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/http/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.881872 hhd-2.7.0/src/hhd/http/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/http/static/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/http/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.881872 hhd-2.7.0/src/hhd/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.865872 hhd-2.7.0/src/hhd/i18n/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.881872 hhd-2.7.0/src/hhd/i18n/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-05-03 12:17:22.000000 hhd-2.7.0/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    22062 2024-05-03 12:17:22.000000 hhd-2.7.0/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.865872 hhd-2.7.0/src/hhd/i18n/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.881872 hhd-2.7.0/src/hhd/i18n/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-03 12:17:22.000000 hhd-2.7.0/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-03 12:17:22.000000 hhd-2.7.0/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.885872 hhd-2.7.0/src/hhd/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.885872 hhd-2.7.0/src/hhd/plugins/display/
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/display/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/gyro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/outputs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.885872 hhd-2.7.0/src/hhd/plugins/overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/overlay/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/overlay/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/overlay/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13232 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/overlay/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.885872 hhd-2.7.0/src/hhd/plugins/powerbutton/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/powerbutton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/powerbutton/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/powerbutton/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/powerbutton/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/touchpad.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/sections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 12:17:15.000000 hhd-2.7.0/src/hhd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.889871 hhd-2.7.0/src/hhd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15418 2024-05-03 12:17:24.000000 hhd-2.7.0/src/hhd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-03 12:17:24.000000 hhd-2.7.0/src/hhd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:17:24.000000 hhd-2.7.0/src/hhd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-03 12:17:24.000000 hhd-2.7.0/src/hhd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 12:17:24.000000 hhd-2.7.0/src/hhd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 12:17:24.000000 hhd-2.7.0/src/hhd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.865872 hhd-2.7.0/usr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.869871 hhd-2.7.0/usr/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.885872 hhd-2.7.0/usr/lib/modules-load.d/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 12:17:15.000000 hhd-2.7.0/usr/lib/modules-load.d/hhd-user.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.869871 hhd-2.7.0/usr/lib/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.885872 hhd-2.7.0/usr/lib/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 12:17:15.000000 hhd-2.7.0/usr/lib/systemd/system/hhd@.service
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 12:17:15.000000 hhd-2.7.0/usr/lib/systemd/system/hhd_local@.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.885872 hhd-2.7.0/usr/lib/systemd/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 12:17:15.000000 hhd-2.7.0/usr/lib/systemd/user/hhd-user.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.869871 hhd-2.7.0/usr/lib/udev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.885872 hhd-2.7.0/usr/lib/udev/hwdb.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-03 12:17:15.000000 hhd-2.7.0/usr/lib/udev/hwdb.d/83-hhd.hwdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:17:24.889871 hhd-2.7.0/usr/lib/udev/rules.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-03 12:17:15.000000 hhd-2.7.0/usr/lib/udev/rules.d/83-hhd-user.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-03 12:17:15.000000 hhd-2.7.0/usr/lib/udev/rules.d/83-hhd.rules
```

### Comparing `hhd-2.6.5/LICENSE` & `hhd-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/PKG-INFO` & `hhd-2.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.6.5
+Version: 2.7.0
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -33,291 +33,180 @@
 <!-- [![]()]() -->
 
 # Handheld Daemon
 Handheld Daemon is a project that aims to provide utilities for managing handheld
 devices.
 It features a fully functional controller emulator that exposes gyro,
 paddles, LEDs and QAM across Steam, RPCS3, Dolphin and others.
-In addition, it features TDP controls for Ryzen devices (beta) and manufacturer
-TDP controls for the Legion Go.
+In addition, it features TDP controls all Ryzen devices and bespoke manufacturer
+controls for the Legion Go and ROG Ally.
 It brings all supported devices up to parity with Steam Deck.
 Read [supported devices](#supported-devices) to see if your device is supported.
 
-Handheld Daemon exposes configuration through an API, and there is already a Decky
-plugin for it ([hhd-decky](https://github.com/hhd-dev/hhd-decky)) and a steam
-overlay, web app for it ([hhd.dev](https://hhd.dev)) that also works locally with Electron
+Handheld Daemon exposes configuration through an API, with a gamemode overlay
+(double press/hold Side Menu), Decky plugin ([hhd-decky](https://github.com/hhd-dev/hhd-decky)),
+web app ([hhd.dev](https://hhd.dev)) and desktop app
 ([hhd-ui](https://github.com/hhd-dev/hhd-ui)).
 
 *Current Features*:
-- Fully functional DualSense and Dualsense Edge emulation
-    - All buttons supported
-    - Rumble feedback
-    - Touchpad support (Steam Input as well)
-    - LED remapping
-- Xbox 360 Style device emulation
+- DualSense and Dualsense Edge emulation
+  - All buttons supported
+  - Rumble feedback
+  - Touchpad support (Steam Input as well)
+  - LED remapping
+- Xbox Elite emulation
   - No weird glyphs
-  - Gyro and back button support (outside Steam)
+  - Back button support
+- Complete SDL UInput Emulation
+  - Joycon (Left, Right, Pair), Switch Pro, Dualsense (Edge), Xbox One, Xbox Series X, Xbox 360
+  - Gyro + Paddles for all SDL apps 
   - Dual Evdev Motion Controllers for Legion Go
 - Virtual Touchpad Emulation
-  - Fixes left and right clicks within gamescope when using the device touchpad.
+  - Fixes left and right clicks within gamemode when using the device touchpad.
 - Power Button plugin for Big Picture/Steam Deck Mode
   - Short press makes Steam backup saves and wink before suspend.
   - Long press opens Steam power menu.
 - TDP Controls ([adjustor](https://github.com/hhd-dev/adjustor))
-- Fully Featured Steam Overlay
-- UI based Configuration
-  - Generic API that can be used from bash scripts (through `curl`)
-  - Decky Plugin
-  - Gamemode Overlay, web app, and desktop app
+  - For ROG Ally and Legion Go: 
+    - TDP, Fan Curves, Charge Limiting the Asus and Lenovo way
+    - Asus: Kernel Driver
+    - Lenovo: acpi_call while the kernel driver is being developed
+  - For Other Devices without firmware TDP controls:
+    - acpi_call + AMD's official manufacturer TDP ACPI bindings
+    - Ayaneo, Ayn, GPD, OneXPlayer
+- Configuration:
+  - Fully Featured Gamemode (Gamescope) Overlay
+  - Desktop App
+  - Web app
+  - Config files
 - Built-in updater.
 
 ## Showcase
 ![Overlay](./docs/overlay.gif)
 
 ## <a name="devices"></a>Supported Devices
-The following devices have been verified to work correctly, with QAM, 
+The following devices have been verified to work correctly, with TDP, QAM, 
 Paddles/extra buttons, RGB remapping, Touchpad, and Gyro support.
 The gyro axis might be incorrect for some of those devices, and can be easily
 fixed in the configuration menu by following [these steps](#axis).
 If you do take the time, please open an issue with the correct mapping so it
 is added to your device.
 
 - Legion Go
 - ROG Ally
 - GPD Win 
-  - Win 4
+  - Win 4 (No LEDs)
   - Win Mini
   - Win Max 2 2023
 - Ayaneo
   - Air Standard/Plus/Pro
   - 1S/1S Limited
   - 2/2S 
   - GEEK, GEEK 1S 
   - NEXT Lite/Pro/Advance
   - SLIDE
+  - 2021 Standard/Pro/Pro Retro Power
+  - NEO 2021/Founder
 - Ayn
   - Loki Zero/Max
 - AOKZOE
-  - A1
-  - A1 Pro 
+  - A1 Normal/Pro (No LEDs)
 - Onexplayer
   - Mini Pro
 
 In addition, Handheld Daemon will attempt to work on Ayaneo, Ayn, Onexplayer, and 
 GPD Win devices that have not been verified to work 
 (controller emulation will be off on first start).
 If everything works and you fix the gyro axis for your device, open an issue
 so that your device can be added to the supported list.
 The touchpad will not work for devices not on the supported list.
 
-RGB support is not yet available for GPD Win 4, it is currently being investigated.
-In addition, GPD Win 4's touch point acts like a mouse, so it unfortunately can not
-be used for steam input.
-Some devices do not support holding the power button to open steam settings on
-the current version, this will be fixed in a future release.
-
 ## Installation Instructions
-You can install the latest stable version of `hhd` from PyPi (recommended), AUR,
-or COPR.
-The easiest way to use Handheld Daemon is to install Bazzite which
-comes pre-installed with the latest version and all required kernel
-fixes for supported devices, see [here](#bazzite).
-Nobara also packages hhd and it will become the default for supported devices soon.
-However, it only packages fixes for the Ally and Legion Go at the time of this
-writing.
-
-> [!IMPORTANT]
-> To ensure the gyro of the Legion Go with AMD SFH runs smoothly, 
-> a udev rule is included that disables the use of the accelerometer by the 
-> system (e.g., iio-sensor-proxy).
-> If you want display auto rotation to work, see manual local steps.
-
-### Automatic Local Install
-You can use the following bash scripts to install and uninstall Handheld Daemon.
-Then, update from Decky or the UI.
-These steps do not work on Bazzite, see [here](#bazzite).
-
+Use the following script to install Handheld Daemon or find your OS [here](#os-install):
 ```bash
-# Install
 curl -L https://github.com/hhd-dev/hhd/raw/master/install.sh | sh
-
-# Uninstall
-curl -L https://github.com/hhd-dev/hhd/raw/master/uninstall.sh | sh
-```
-
-You can also install the Decky plugin.
-Having Decky installed is a prerequisite ([instructions](https://github.com/SteamDeckHomebrew/decky-loader#-installation)).
-```bash
-curl -L https://github.com/hhd-dev/hhd-decky/raw/main/install.sh | sh
 ```
 
-Then, reboot and go to [hhd.dev](https://hhd.dev) to configure or read more in
-the [configuration section](#configuration).
+You can use this script on NobaraOS (after uninstalling the built-in Handheld Daemon/HandyGCCS).
+ChimeraOS up to 45-1 is not supported due to general instability (uninstall HandyGCCS if you do).
+This does not work and is not needed on Bazzite, see [here](#bazzite).
+
+> [!IMPORTANT]  
+> For non-gaming distros, see [here](./kernel.md) for a partial list of kernel 
+> patches. This includes `acpi_call` for TDP on devices other than the Ally.
 
-> [!IMPORTANT]
-> Before creating an issue, make sure you are using the latest Handheld Daemon 
-> version and that you read the extra information for each setting in 
-> either [hhd.dev](https://hhd.dev) or the `state.yml` file.
-> 
-> The context is required to understand what each setting does and is 
-> not included in the current version of the Decky Plugin 
-> due to UI limitations.
-
-#### Using an older version
-If you find any issues with the latest version of Handheld Daemon
-you can use any version by specifying it with the command below.
+You can also install the Decky plugin (optional; decky required):
+([instructions](https://github.com/SteamDeckHomebrew/decky-loader#-installation)):
 ```bash
-sudo systemctl stop hhd_local@$(whoami)
-~/.local/share/hhd/venv/bin/pip install hhd==1.0.6
-sudo systemctl start hhd_local@$(whoami)
+curl -L https://github.com/hhd-dev/hhd-decky/raw/main/install.sh | sh
 ```
 
-### Manual Local Installation
-You can also install Handheld Daemon using a local package, which enables auto-updating.
-These are the same steps as done in the Automatic Install (also see 
-[Common Issues after Install](#issues)).
-These steps do not work on Bazzite, see [here](#bazzite).
-
+### Uninstall
+We are sorry to see you go, use the following to uninstall:
 ```bash
-# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-# !!!! Uninstall HandyGCCS to avoid issues if you have it. !!!!
-# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-
-# Install Handheld Daemon to ~/.local/share/hhd
-mkdir -p ~/.local/share/hhd && cd ~/.local/share/hhd
-
-python3 -m venv --system-site-packages venv
-source venv/bin/activate
-pip install --upgrade hhd adjustor
-# Substitute with the following to pull from github (may not always work)
-# pip install git+https://github.com/hhd-dev/hhd git+https://github.com/hhd-dev/hhd-ui
-
-# Install the UI to ~/.local/bin
-FINAL_URL='https://api.github.com/repos/hhd-dev/hhd-ui/releases/latest'
-curl -L $(curl -s "${FINAL_URL}" | grep "browser_download_url" | cut -d '"' -f 4) -o $HOME/.local/bin/hhd-ui
-chmod +x $HOME/.local/bin/hhd-ui
-
-# Install udev rules and create a service file
-sudo curl https://raw.githubusercontent.com/hhd-dev/hhd/master/usr/lib/udev/rules.d/83-hhd.rules -o /etc/udev/rules.d/83-hhd.rules
-sudo curl https://raw.githubusercontent.com/hhd-dev/hhd/master/usr/lib/udev/hwdb.d/83-hhd.hwdb -o /etc/udev/hwdb.d/83-hhd.hwdb
-sudo curl https://raw.githubusercontent.com/hhd-dev/hhd/master/usr/lib/systemd/system/hhd_local%40.service -o /etc/systemd/system/hhd_local@.service
-
-# Change rules to re-enable display autorotation if you do not want gyro support.
-# sudo nano /etc/udev/rules.d/83-hhd.rules
-
-# Start service and reboot
-sudo systemctl enable hhd_local@$(whoami)
-sudo reboot
+curl -L https://github.com/hhd-dev/hhd/raw/master/uninstall.sh | sh
 ```
 
-#### Using an older version
+### Using an older version
 If you find any issues with the latest version of Handheld Daemon
 you can use any version by specifying it with the command below.
 ```bash
 sudo systemctl stop hhd_local@$(whoami)
-~/.local/share/hhd/venv/bin/pip install hhd==1.0.6
+~/.local/share/hhd/venv/bin/pip install hhd==2.6.0
 sudo systemctl start hhd_local@$(whoami)
 ```
 
-#### Update Instructions
-Of course, you will want to update Handheld Daemon to catch up to latest features.
-You can either use the commands below or press `Update (Stable)` in one of the UIs
-(which runs these commands).
-```bash
-sudo systemctl stop hhd_local@$(whoami)
-~/.local/share/hhd/venv/bin/pip install --upgrade hhd
-sudo systemctl start hhd_local@$(whoami)
-```
-
-#### Uninstall instructions
-To uninstall, simply stop the service and remove the added files.
-```bash
-sudo systemctl disable hhd_local@$(whoami)
-sudo systemctl stop hhd_local@$(whoami)
-
-rm -rf ~/.local/share/hhd
-rm -f ~/.local/bin/hhd-ui
-sudo rm /etc/udev/rules.d/83-hhd.rules
-sudo rm /etc/udev/hwdb.d/83-hhd.hwdb
-sudo rm /etc/systemd/system/hhd_local@.service
-
-# Delete your configuration
-rm -r ~/.config/hhd
-```
-### <a name="gyro"></a>Kernel Patches
-There is an optional kernel patch for the Legion Go that increases the Display
-Gyro accuracy [here](https://github.com/hhd-dev/linux-handheld/blob/master/6.6/0001-amd-sfh-bump-sensitivity.patch).
-
-For LED support, the following modules are required for Ayaneo and Ayn: 
-[ayaneo-platform](https://github.com/ShadowBlip/ayaneo-platform)
-driver, and for Ayn, the [ayn-platform](https://github.com/ShadowBlip/ayn-platform).
-Provided these drivers are installed and are supported by your device,
-LED support will be enabled by default.
-
-### Gyro
-Which kernel patch is required will depend on your device's bosch module.
-For the Bosch 260 IMU, you will need the 
-[bmi260-dkms](https://github.com/hhd-dev/bmi260) driver.
-For the Bosch 160 IMU and certain devices, you will need the following bmi160
-[kernel patch](https://github.com/pastaq/bmi160-aya-neo/blob/main/bmi160_ayaneo.patch).
-Ayaneo Air Plus and Ally use the Bosch 323 and need the patch series from
-this repository: [Ally Nobara Fixes](https://github.com/jlobue10/ALLY_Nobara_fixes). 
-The Legion Go does not need kernel patches.
-
-In addition, for most devices, your kernel config should also 
-enable the modules `SYSFS trigger` with `CONFIG_IIO_SYSFS_TRIGGER` and
-`High resolution timer trigger` with `CONFIG_IIO_HRTIMER_TRIGGER`.
-Both are under `Linux Kernel Configuration ─> Device Drivers ─> Industrial I/O support ─> Triggers - standalone`.
-
 ### <a name="issues"></a>After Install Instructions
 #### Extra steps for ROG Ally
-Without an up-to-date `asus-wmi` kernel driver the usb device of the controller
-does not wake up after sleep so Handheld Daemon stops working.
-This patch is included with Linux kernel 6.7.
 You can hold the ROG Crate button to switch to the ROG Ally's Mouse mode to turn
 the right stick into a mouse.
 
+Combinations with the ROG, Armory Crate buttons is not supported in the Ally,
+you can swap them with start/select for this functionality.
+
 #### Extra steps GPD Win Devices
 In order for the back buttons in GPD Win Devices to work, you need to map the
-back buttons to Left: Printscreen, Right: Pause using Windows.
+back buttons to Left: PrintScreen, Right: Pause using Windows.
 This is the default mapping, so if you never remapped them using Windows you
 will not have to.
 Handheld Daemon automatically handles the interval to enable being able to hold
 the buttons.
 
 Here is how the button settings should look:
 ```
 Left-key: PrtSc + 0ms + NC + 0ms + NC + 0ms + NC
 Right-key: Pausc + 0ms + NC + 0ms + NC + 0ms + NC
 ```
 
-Unfortunately, its not possible to rapid double tap the buttons due to their
+Unfortunately, it is not possible to rapid double tap the buttons due to their
 implementation.
 The R4 button is mapped to Side Menu (QAM) by default.
 
 #### Extra steps for Ayaneo/Ayn/Onexplayer
-You might experience a tiny amount of lag with the Ayaneo LEDs
+You might experience a tiny amount of lag with the Ayaneo LEDs.
 The paddles of the Ayn Loki Max are not remappable as far as we know.
 
 #### Extra steps for Legion Go
-If you are using a kernel older than 6.8 and you are not on a gaming distro
-(ChimeraOS, Nobara, Bazzite), you need the following rule for the controllers
+If you have set any mappings on Legion Space, they will interfere with Handheld
+Daemon.
+You can factory reset the Controllers from the Handheld Daemon settings.
+
+The controller gyros of the Legion Go tend to drift and have noise.
+However, they are excellent after calibration.
+Calibrate them using steam calibration and be patient, as they will fail a lot.
+Depending on their state in rare cases they might not be possible to calibrate.
+
+If you are using a kernel older than 6.8, and you are not on a gaming distro
+(Nobara, Bazzite), you need the following rule for the controllers
 to be recognized.
 ```bash
 # Enable xpad for the Legion Go controllers
 ATTRS{idVendor}=="17ef", ATTRS{idProduct}=="6182", RUN+="/sbin/modprobe xpad" RUN+="/bin/sh -c 'echo 17ef 6182 > /sys/bus/usb/drivers/xpad/new_id'"
 ```
 
-If you have set any mappings on Legion Space, they will interfere with Handheld
-Daemon.
-As of version 2.0.0, you can factory reset the controllers from the Handheld
-Daemon settings, or you
-can partially reset them controllers by holding Legion R + RT + RB, 
-and then Legion L + LT + LB or booting into windows.
-
 #### High Touchpad Sensitivity in Steam Input
 By default, the Dualsense kernel driver exposes the Dualsense trackpad as a normal
 trackpad.
 This means that if you go to use it as steam input, you still get the normal
 trackpad input.
 This leads to double input.
 
@@ -330,183 +219,105 @@
 ACTION=="add|change", KERNEL=="event[0-9]*", ATTRS{name}=="*Wireless Controller Touchpad", ENV{LIBINPUT_IGNORE_DEVICE}="1"
 ```
 
 The package `ds-inhibit` is available in AUR, packaged for Nobara, and enabled
 by default in Bazzite.
 
 #### Playstation Glyphs and Controller Image
-If you do not want playstation glyphs in Steam, you can use https://github.com/frazse/PS5-to-Xbox-glyphs
+If you do not want Playstation glyphs in Steam, you can use 
+https://github.com/frazse/PS5-to-Xbox-glyphs
 as a CSS Loader plugin to switch them to Xbox.
 Then, there are CSS plugins for the Legion Go and Ally controller images in
 https://github.com/frazse/SBP-Legion-Go-Theme and 
 https://github.com/semakusut/SBP-ROG-Ally respectively.
-If you are using Bazzite, you can also find a `ujust` version of the commands in 
-the Bazzite readme.
+If you are using Bazzite, you can also find a `ujust` version of the commands 
+in the Bazzite readme.
 
-#### Missing Python Evdev
-In case you have installation issues, you might be missing the package `python-evdev`.
-You can either install it as part of your distribution (included by Nobara
-and ChimeraOS) or automatically through `pip` with the commands above.
-However, installing this package through `pip` requires `base-devel` on Arch and
-`python-devel` on Nobara.
-```bash
-# Nobara/Fedora
-sudo dnf install python-evdev
-# Arch based distros (included by ChimeraOs)
-sudo pacman -S python-evdev
-
-# OR
-
-# (nobara) Install Python Headers since evdev has no wheels
-# and nobara does not ship them (but arch does)
-sudo dnf install python-devel
-# (Chimera, Arch) In case you dont have gcc.
-sudo pacman -S base-devel
-```
+## <a name="configuration"></a>Configuration
+Open the overlay (double press side button), or open the desktop app (`Handheld Daemon`/`$ hhd-ui`),
+or go to [hhd.dev](https://hhd.dev) and enter your device token (`~/.config/hhd/token`).
+Then just start configuring!
 
-#### Having HandyGCCS Installed
-If your distro ships with HandyGCCS Handheld Daemon will not work, you have to uninstall it.
-```bash
-# ChimeraOS
-sudo frzr-unlock
-sudo systemctl disable --now handycon.service
-sudo pacman -R handygccs-git
-
-# Nobara
-sudo systemctl disable --now handycon.service
-sudo dnf remove handygccs-git # (verify ?)
+You can also use the Decky plugin (needs Decky):
 ```
-
-### <a name="bazzite"></a><a name="after-install"></a>Bazzite
-Handheld Daemon comes pre-installed on Bazzite and updates along-side the system.
-The latest version of Handheld Daemon becomes available at the latest the next
-day after release, and can be managed through the Bazzite updater.
-In addition, Bazzite contains all the required kernel patches for the Handheld Daemon
-supported devices, so it is the recommended distro to use Handheld Daemon with.
-
-After install, you can use `ujust` to install Decky and the Handheld Daemon Decky
-plugin with the commands `ujust setup-decky`, `ujust setup-decky hhd-decky`.
-
-If you need to use a different Handheld Daemon version or a custom one, the 
-install steps do not currently work for Bazzite, but this will be fixed in the future.
-Essentially, a new service file needs to be written for Bazzite that contains the
-correct home path (`/var/home`) and then you can disable the built-in version
-service and use the new one instead.
-
-See [supported devices](#supported-devices) to check the status of your device and 
-[after install](#issues) for specific device quirks.
-
-### ❄️ NixOS
-Ensure your `nixpkgs` is on the `unstable` channel (as of Feb 2024):
-
-```nix
-  inputs = {
-    nixpkgs.url = "github:nixos/nixpkgs/nixos-unstable";
+curl -L https://github.com/hhd-dev/hhd-decky/raw/main/install.sh | sh
 ```
 
-and add this line to your `configuration.nix`:
-```nix
-  services.handheld-daemon.enable = true;
-```
+The configuration files are stored under `~/.config/hhd` with the main one being
+`state.yml`, which can be edited and will hot reload.
 
-### Distribution Installation (not recommended)
+## <a name="os-install"></a> Distribution Install
 You can install Handheld Daemon from [AUR](https://aur.archlinux.org/packages/hhd) 
 (Arch) or [COPR](https://copr.fedorainfracloud.org/coprs/hhd-dev/hhd/) (Fedora).
 Both update automatically every time there is a new release.
 
 But, the auto-updater will not work, which is an important feature with devices
 without a keyboard.
 ```bash
 # Arch
-yay -S hhd hhd-ui adjustor
+yay -S hhd adjustor hhd-ui
 
 # Fedora
 sudo dnf copr enable hhd-dev/hhd
-sudo dnf install hhd adjustor
-# HHD-UI todo
+sudo dnf install hhd adjustor hhd-ui
 
-# Enable and reboot
 sudo systemctl enable hhd@$(whoami)
-sudo reboot
 ```
 
-In case you do not want to reboot.
-```bash
-# Reload Handheld Daemon's udev rules
-sudo udevadm control --reload-rules && sudo udevadm trigger
-# Restart iio-proxy-service to stop it
-# from polling the accelerometer
-sudo systemctl restart iio-sensor-proxy
-# Start the service for your user
-sudo systemctl start hhd@$(whoami)
-```
+### ❄️ NixOS
+Handheld Daemon (core; no overlay, TDP) is on `nixpkgs` in the `unstable` channel.
 
-## <a name="configuration"></a>Configuration
-### UI Based
-Go to [hhd.dev](https://hhd.dev) and enter your device token 
-(`~/.config/hhd/token`).
-That is it!
-You can also install the Electron version ([hhd-ui](https://github.com/hhd-dev/hhd-ui)) 
-to use completely offline or as an app (updating it has to be done manually for now).
-
-### Using Decky
-If you have decky installed, you can use the following command to
-install the Handheld Daemon decky plugin (visit 
-[hhd-decky](https://github.com/hhd-dev/hhd-decky) for details).
-```
-curl -L https://github.com/hhd-dev/hhd-decky/raw/main/install.sh | sh
+Add the following to your `configuration.nix` to enable:
+```nix
+  services.handheld-daemon.enable = true;
+  services.handheld-daemon.user = "<your-user>";
 ```
-Then, just open up steam.
 
-### File based
-The reason you added your username to the `hhd` service was to bind the `hhd`
-daemon to your user.
+### <a name="bazzite"></a><a name="after-install"></a>Bazzite
+Handheld Daemon comes pre-installed on [Bazzite](https://bazzite.gg) and 
+updates along-side the system.
+Most users of Handheld Daemon are on Bazzite and Bazzite releases
+often happen to bundle Handheld Daemon.
+Bazzite contains all kernel patches and quirks required for all supported handhelds
+to work (to the extent they can; certain Ayaneo devices have issues.)
 
-This allows Handheld Daemon to add configuration files with appropriate
-permissions to your user, in the following directory:
-```bash
-~/.config/hhd
-```
+After install, you can use `ujust` to install Decky and the Handheld Daemon Decky
+plugin with the commands `ujust setup-decky`, `ujust setup-decky hhd-decky`.
 
-The global configuration for HHD is found in:
-```bash
-~/.config/hhd/state.yml
-```
+If you need to use a different Handheld Daemon version or a custom one, the 
+install steps do not currently work for Bazzite, a `ujust` command is in the works.
 
-You can modify it and it will hot-reload upon saving.
+See [supported devices](#supported-devices) to check the status of your device and 
+[after install](#issues) for specific device quirks.
 
 ## Contributing
 ### <a name="axis"></a> Finding the correct axis for your device
-To figure the correct axis from your device, go to desktop and open the steam
-calibration settings.
-Then, go to https://hhd.dev , switch `Motion Axis` to `Override` and tweak only
-the axis (without invert) of your device until they match the glyphs in steam.
-
-> [!WARNING]  
-> Do not try to interpret what each axis means. You will get a headache. 
-> Just change them randomly until
-> the glyphs line up with how you move your controller.
-> If you set multiple axis to a single one (e.g., X to Y, and Y to Y),
-> the first option (e.g., X to Y) option will be ignored.
+To figure the correct axis from your device, go to steam calibration settings.
+Then, in the overlay (double press/hold side button) switch `Motion Axis` to 
+`Override` and tweak only the axis (without invert) of your device until they 
+match the glyphs in steam.
 
 Then, jump in a first person game and turn on `Gyro to Mouse` or `Camera`.
-For `Gyro to Mouse`, use `Gyro to Mouse fix` if you get issues with the camera
-jumping around.
-By default, rotating your device like a steering wheel should turn left to right,
+By default (`Yaw`), rotating your device like a steering wheel should turn left 
+to right,
 and rotating it to face down or up should look up or down.
 Fix the invert settings of the axis so that it is intuitive.
 Finally, switch the setting `Gyro Turning Axis` from `Yaw` (rotate like a steering
 wheel) to `Roll` (turn left to right), and fix the remaining axis inversion.
 
 You can now either take a picture of your screen or translate the settings into
 text (e.g., x is k, y is l inverted, z is j) and open an issue.
 The override setting also displays the make and model of your device, which
 are required to add the mappings to Handheld Daemon.
 
 ### Localizing Handheld Daemon
+Handheld Daemon fully supports localization through standard `PO`, `POT` files.
+Contribution instructions in progress!!!
+
+#### For maintainers
 You can find `pot` and `po` files for Handheld Daemon under the `i18n` directory.
 You can clone/download this repository and open the `./i18n` directory.
 Then, just copy the `*.pot` files into `<your_locale>/LC_MESSAGES/*.po`
 and begin translating with your favorite text editor, or by using
 tool such as [Lokalize](https://apps.kde.org/lokalize/).
 
 As far as your locale goes, unless you have a good reason to, skip the territory
```

### Comparing `hhd-2.6.5/pyproject.toml` & `hhd-2.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hhd"
-version = "2.6.5"
+version = "2.7.0"
 authors = [
   { name="Kapenekakis Antheas", email="pypi@antheas.dev" },
 ]
 description = "Handheld Daemon, a tool for configuring handheld devices."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `hhd-2.6.5/src/hhd/__main__.py` & `hhd-2.7.0/src/hhd/__main__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/contrib/dev.py` & `hhd-2.7.0/src/hhd/contrib/dev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/contrib/gs.py` & `hhd-2.7.0/src/hhd/contrib/gs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/contrib/i18n.py` & `hhd-2.7.0/src/hhd/contrib/i18n.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/contrib/main.py` & `hhd-2.7.0/src/hhd/contrib/main.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/__init__.py` & `hhd-2.7.0/src/hhd/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/base.py` & `hhd-2.7.0/src/hhd/controller/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,15 +325,15 @@
 
     def close(self, exit: bool) -> bool:
         """Called to close the device.
 
         If `exit` is true, the program is about to
         close. If it is false, the controller may be performing a configuration
         change.
-        
+
         In the first versions of Handheld Daemon, this API was meant to be used
         for the controller to enter power saving mode. However, it turns out
         that steam and the kernel do not let the controller disconnect,
         so it was repurposed to skip controller hiding."""
         return False
 
     def produce(self, fds: Sequence[int]) -> Sequence[Event]:
@@ -429,14 +429,15 @@
         self.qam_multi_tap = qam_multi_tap and not os.environ.get(
             "HHD_QAM_MULTI_DISABLE", None
         )
         self.guide_pressed = False
         self.steam_check = params.get("steam_check", None)
         self.steam_check_last = time.perf_counter()
         self.steam_check_fn = params.get("steam_check_fn", None)
+        self.nintendo_qam = params.get("nintendo_qam", False)
 
         self.unique = str(time.perf_counter_ns())
         assert touchpad is None, "touchpad rewiring not supported yet"
 
     def process(self, events: Sequence[Event]):
         out: list[Event] = []
         status_events = set()
@@ -913,25 +914,25 @@
                         "value": True,
                     },
                 )
                 self.queue.append(
                     (
                         {
                             "type": "button",
-                            "code": "a",
+                            "code": "b" if self.nintendo_qam else "a",
                             "value": True,
                         },
                         curr + self.QAM_DELAY,
                     )
                 )
                 self.queue.append(
                     (
                         {
                             "type": "button",
-                            "code": "a",
+                            "code": "b" if self.nintendo_qam else "a",
                             "value": False,
                         },
                         curr + 2 * self.QAM_DELAY,
                     ),
                 )
                 self.queue.append(
                     (
```

### Comparing `hhd-2.6.5/src/hhd/controller/const.py` & `hhd-2.7.0/src/hhd/controller/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/lib/common.py` & `hhd-2.7.0/src/hhd/controller/lib/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 buff[t.loc >> 3 : (t.loc >> 3) + 1], t.order, signed=False
             )
             s = (1 << 8) - 1
         case "m8":
             o = int.from_bytes(
                 buff[t.loc >> 3 : (t.loc >> 3) + 1], t.order, signed=False
             ) - (1 << 7)
-            s = (1 << 7) - 1
+            s = (1 << 7)
         case _:
             assert False, f"Invalid formatting {t.type}."
 
     if t.scale:
         v = t.scale * o + t.offset
     else:
         v = o / s + t.offset
```

### Comparing `hhd-2.6.5/src/hhd/controller/lib/hid.py` & `hhd-2.7.0/src/hhd/controller/lib/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/lib/hide.py` & `hhd-2.7.0/src/hhd/controller/lib/hide.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import subprocess
 import os
+# import re
 
 
 def get_syspath(devpath: str):
     for line in subprocess.run(
         ["udevadm", "info", devpath], capture_output=True
     ).stdout.splitlines():
         if line.startswith(b"P: "):
@@ -27,14 +28,15 @@
 
 def get_parent_sysfs(devpath: str):
     syspath = get_syspath(devpath)
     if not syspath:
         return None
 
     return syspath[: syspath.rindex("/")]
+    # return syspath.split("/input/")[0]
 
 
 def reload_children(parent: str):
     stat = subprocess.run(
         ["udevadm", "control", "--reload-rules"],
         capture_output=True,
     )
@@ -65,15 +67,26 @@
 # Hides device gamepad devices stemming from {input_dev}
 # Managed by HHD, this file will be autoremoved during configuration changes.
 SUBSYSTEMS=="input", KERNELS=="{input_dev}", ATTRS{{id/vendor}}=="{vid:04x}", ATTRS{{id/product}}=="{pid:04x}", GOTO="hhd_valid"
 GOTO="hhd_end"
 LABEL="hhd_valid"
 KERNEL=="js[0-9]*|event[0-9]*", SUBSYSTEM=="input", MODE="000", GROUP="root", TAG-="uaccess", RUN+="/bin/chmod 000 /dev/input/%k"
 LABEL="hhd_end"
-"""  # , RUN+="/bin/chmod 000 /sys/%p"
+"""
+
+#     # Hide usb xinput, be very careful to only match that usb
+#     if "/" in parent:
+#         usb_root = parent[parent.rindex("/") + 1 :]
+#         if re.match(r"\d-+\d+", usb_root) or re.match(r"\d+-\d+:\d+\.\d+", usb_root):
+#             rule += f"""
+# # Hides the Xinput/Hidraw input node so that certain games that access it directly.
+# SUBSYSTEMS=="usb", ATTRS{{idVendor}}=="{vid:04x}", ATTRS{{idProduct}}=="{pid:04x}",\
+#  KERNEL=="{usb_root}", TAG-="uaccess", GROUP="root", MODE="000"
+# """
+
     try:
         os.makedirs("/run/udev/rules.d/", exist_ok=True)
         with open(out_fn, "w") as f:
             f.write(rule)
         reload_children(parent)
         return input_dev
     except Exception:
```

### Comparing `hhd-2.6.5/src/hhd/controller/lib/ioctl.py` & `hhd-2.7.0/src/hhd/controller/lib/ioctl.py`

 * *Files 5% similar despite different names*

```diff
@@ -228,18 +228,22 @@
 # struct input_mask {
 # 	__u32 type;
 # 	__u32 codes_size;
 # 	__u64 codes_ptr;
 # };
 EVIOCGMASK = _IOR("E", 0x92, 4 + 4 + 8)
 EVIOCSMASK = _IOW("E", 0x93, 4 + 4 + 8)
-
+# char * is 8
+UINPUT_IOCTL_BASE = "U"
+UI_SET_UNIQ_STR = lambda l: _IOC("w", UINPUT_IOCTL_BASE, 112, l)
+UI_GET_SYSNAME = lambda l: _IOC("r", UINPUT_IOCTL_BASE, 44, l)
 
 __all__ = (
     "_IOC",
     "_IO",
     "_IOR",
     "_IOW",
     "_IOWR",
     "EVIOCSMASK",
     "EVIOCGMASK",
+    "UI_SET_UNIQ_STR",
 )
```

### Comparing `hhd-2.6.5/src/hhd/controller/lib/uhid.py` & `hhd-2.7.0/src/hhd/controller/lib/uhid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/physical/evdev.py` & `hhd-2.7.0/src/hhd/controller/physical/evdev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/physical/hidraw.py` & `hhd-2.7.0/src/hhd/controller/physical/hidraw.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/physical/imu.py` & `hhd-2.7.0/src/hhd/controller/physical/imu.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     dev: str
     axis: Sequence[ScanElement]
     sysfs: str
 
 
 ACCEL_NAMES = ["accel_3d"]
 GYRO_NAMES = ["gyro_3d"]
-IMU_NAMES = ["bmi323-imu", "BMI0160", "BMI0260"]
+IMU_NAMES = ["bmi323-imu", "BMI0160", "BMI0260", "i2c-10EC5280:00"]
 SYSFS_TRIG_CONFIG_DIR = os.environ.get("HHD_MOUNT_TRIG_SYSFS", "/var/trig_sysfs_config")
 
 ACCEL_MAPPINGS: dict[str, tuple[Axis, str | None, float, float | None]] = {
     "accel_x": ("accel_z", "accel", 1, None),
     "accel_y": ("accel_x", "accel", 1, None),
     "accel_z": ("accel_y", "accel", 1, None),
     "timestamp": ("accel_ts", None, 1, None),
```

### Comparing `hhd-2.6.5/src/hhd/controller/physical/rgb.py` & `hhd-2.7.0/src/hhd/controller/physical/rgb.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/virtual/dualsense/__init__.py` & `hhd-2.7.0/src/hhd/controller/virtual/dualsense/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/virtual/dualsense/const.py` & `hhd-2.7.0/src/hhd/controller/virtual/dualsense/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/virtual/sd/__init__.py` & `hhd-2.7.0/src/hhd/controller/virtual/sd/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/virtual/sd/const.py` & `hhd-2.7.0/src/hhd/controller/virtual/sd/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/controller/virtual/uinput/__init__.py` & `hhd-2.7.0/src/hhd/controller/virtual/uinput/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,71 +4,82 @@
 
 from evdev import UInput
 
 from hhd.controller.base import Consumer, Event, Producer, can_read
 from hhd.controller.const import Axis, Button
 
 from .const import *
+from .monkey import UInputMonkey
 
 logger = logging.getLogger(__name__)
 
 
-# Monkey patch Uinput device to avoid issues
-# _find_device() may crash when controllers
-# disconnect. We dont use the produced device anyway.
-def _patch(*args, **kwargs):
-    pass
-
-
-UInput._find_device = _patch
-
-
 class UInputDevice(Consumer, Producer):
-
     def __init__(
         self,
         capabilities=GAMEPAD_CAPABILITIES,
         btn_map: dict[Button, int] = GAMEPAD_BUTTON_MAP,
         axis_map: dict[Axis, AX] = GAMEPAD_AXIS_MAP,
         vid: int = HHD_VID,
         pid: int = HHD_PID_GAMEPAD,
+        bus: int = 0x03,
         name: str = "Handheld Daemon Controller",
         phys: str = "phys-hhd-gamepad",
         output_imu_timestamps: str | bool = False,
         output_timestamps: bool = False,
         input_props: Sequence[int] = [],
         ignore_cmds: bool = False,
+        uniq: str | None = None,
     ) -> None:
         self.capabilities = capabilities
         self.btn_map = btn_map
         self.axis_map = axis_map
         self.dev = None
         self.name = name
         self.vid = vid
         self.pid = pid
+        self.bus = bus
         self.phys = phys
+        self.uniq = uniq
         self.output_imu_timestamps = output_imu_timestamps
         self.output_timestamps = output_timestamps
         self.ofs = 0
         self.sys_ofs = 0
         self.input_props = input_props
         self.ignore_cmds = ignore_cmds
 
         self.rumble: Event | None = None
 
     def open(self) -> Sequence[int]:
         logger.info(f"Opening virtual device '{self.name}'.")
-        self.dev = UInput(
-            events=self.capabilities,
-            name=self.name,
-            vendor=self.vid,
-            product=self.pid,
-            phys=self.phys,
-            input_props=self.input_props,
-        )
+        try:
+            self.dev = UInputMonkey(
+                events=self.capabilities,
+                name=self.name,
+                vendor=self.vid,
+                product=self.pid,
+                bustype=self.bus,
+                phys=self.phys,
+                input_props=self.input_props,
+                uniq=self.uniq,
+            )
+        except Exception as e:
+            logger.error(
+                f"Monkey patch probably failed. Could not create evdev device with uniq:\n{e}"
+            )
+            self.dev = UInput(
+                events=self.capabilities,
+                name=self.name,
+                vendor=self.vid,
+                product=self.pid,
+                bustype=self.bus,
+                phys=self.phys,
+                input_props=self.input_props,
+            )
+
         self.touchpad_aspect = 1
         self.touch_id = 1
         self.fd = self.dev.fd
 
         if self.ignore_cmds:
             # Do not wake up if we ignore to save utilization
             # When the output contains a timestamp, it is fed back to evdev
@@ -84,31 +95,37 @@
         self.fd = None
         return True
 
     def consume(self, events: Sequence[Event]):
         if not self.dev:
             return
 
-        wrote = False
-        for ev in events:
+        wrote = {}
+        ts = 0
+        for ev in reversed(events):
+            key = (ev["type"], ev["code"])
+            if key in wrote:
+                # skip duplicate events that were caused due to a delay
+                # only keep the last button value by iterating reversed
+                continue
             match ev["type"]:
                 case "axis":
                     if ev["code"] in self.axis_map:
                         ax = self.axis_map[ev["code"]]
                         if ev["code"] == "touchpad_x":
                             val = int(
                                 self.touchpad_aspect
                                 * (ax.scale * ev["value"] + ax.offset)
                             )
                         else:
                             val = int(ax.scale * ev["value"] + ax.offset)
                         if ax.bounds:
                             val = min(max(val, ax.bounds[0]), ax.bounds[1])
                         self.dev.write(B("EV_ABS"), ax.id, val)
-                        wrote = True
+                        wrote[key] = val
 
                         if ev["code"] == "touchpad_x":
                             self.dev.write(B("EV_ABS"), B("ABS_MT_POSITION_X"), val)
                         elif ev["code"] == "touchpad_y":
                             self.dev.write(B("EV_ABS"), B("ABS_MT_POSITION_Y"), val)
 
                     elif (
@@ -118,22 +135,17 @@
                             "accel_ts",
                             "gyro_ts",
                             "imu_ts",
                         )
                     ) or ev["code"] == self.output_imu_timestamps:
                         # We have timestamps with ns accuracy.
                         # Evdev expects us accuracy
-                        ts = ev["value"] // 1000
-                        # Use an ofs to avoid overflowing
-                        if ts > self.ofs + 2**30:
-                            self.ofs = ts
-                        ts -= self.ofs
-                        if ts > 0:
-                            self.dev.write(B("EV_MSC"), B("MSC_TIMESTAMP"), ts)
-                        wrote = True
+                        ts = (ev["value"] // 1000) % (2**31)
+                        self.dev.write(B("EV_MSC"), B("MSC_TIMESTAMP"), ts)
+                        wrote[key] = ts
                 case "button":
                     if ev["code"] in self.btn_map:
                         if ev["code"] == "touchpad_touch":
                             self.dev.write(
                                 B("EV_ABS"),
                                 B("ABS_MT_TRACKING_ID"),
                                 self.touch_id if ev["value"] else -1,
@@ -147,31 +159,27 @@
                             if self.touch_id > 500:
                                 self.touch_id = 1
                         self.dev.write(
                             B("EV_KEY"),
                             self.btn_map[ev["code"]],
                             1 if ev["value"] else 0,
                         )
-                        wrote = True
+                        wrote[key] = ev["value"]
 
                 case "configuration":
                     if ev["code"] == "touchpad_aspect_ratio":
                         self.touchpad_aspect = float(ev["value"])
 
         if wrote and self.output_timestamps:
             # We have timestamps with ns accuracy.
             # Evdev expects us accuracy
-            ts = time.perf_counter_ns() // 1000
-            # Use an ofs to avoid overflowing
-            if ts > self.ofs + 2**30:
-                self.ofs = ts
-            ts -= self.ofs
+            ts = (time.perf_counter_ns() // 1000) % (2**31)
             self.dev.write(B("EV_MSC"), B("MSC_TIMESTAMP"), ts)
 
-        if wrote:
+        if wrote and (not self.output_imu_timestamps or ts):
             self.dev.syn()
 
     def produce(self, fds: Sequence[int]) -> Sequence[Event]:
         if self.ignore_cmds or not self.fd or not self.fd in fds or not self.dev:
             return []
 
         out: Sequence[Event] = []
```

### Comparing `hhd-2.6.5/src/hhd/controller/virtual/uinput/const.py` & `hhd-2.7.0/src/hhd/controller/virtual/uinput/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,38 @@
 HHD_PID_GAMEPAD = 0x01
 HHD_PID_KEYBOARD = 0x02
 HHD_PID_MOUSE = 0x03
 HHD_PID_TOUCHPAD = 0x04
 HHD_PID_MOTION = 0x11
 HHD_PID_VENDOR = 0x7000
 
+CONTROLLER_THEMES: dict[str, tuple[int, int, str]] = {
+    "hhd": (0x5335, 0x0001, "Handheld Daemon Controller"),
+    # Sony
+    "ps3": (0x054C, 0x0268, "DualShock 3"),
+    "ps4": (0x054C, 0x05C4, "DualShock 4"),
+    "ps5": (0x054C, 0x0CE6, "DualSense"),
+    "ps5e": (0x054C, 0x0DF2, "DualSense Edge"),
+    # Microsoft
+    "xbox_360": (0x045E, 0x028F, "Xbox 360"),
+    "xbox_one": (0x045E, 0x02D1, "Xbox One"),
+    "xbox_one_elite": (0x045E, 0x02E3, "Xbox Elite"),
+    "xbox_sx": (0x045E, 0x0B12, "Xbox Series X"),
+    # Nintendo
+    "joycon_left": (0x057E, 0x2006, "JoyCon Left"),
+    "joycon_right": (0x057E, 0x2007, "JoyCon Right"),
+    "joycon_pair": (0x057E, 0x2008, "JoyCon Pair"),
+    "joycon_grip": (0x057E, 0x200E, "JoyCon Grip"),
+    "switch_pro": (0x057E, 0x2009, "Switch Pro"),
+    # Valve
+    "steam_deck": (0x28DE, 0x1205, "Steam Deck"),
+    "steam_controller": (0x28DE, 0x1202, "Steam Controller"),
+    "steam_input": (0x28DE, 0x11FF, "Steam Input"),
+}
+
 
 def B(b: str | Sequence[str], num: int | None = None):
     if num is not None:
         return num
     assert b, f"No value provided."
     if not isinstance(b, str):
         b = b[0]
@@ -460,14 +484,23 @@
     "accel_y": AX(B("ABS_Y"), 8192 / 9.8, bounds=(-32768, 32768)),
     "accel_z": AX(B("ABS_Z"), 8192 / 9.8, bounds=(-32768, 32768)),
     "gyro_x": AX(B("ABS_RX"), 1024 * 180 / 3.14, bounds=(-2097152, 2097152)),
     "gyro_y": AX(B("ABS_RY"), 1024 * 180 / 3.14, bounds=(-2097152, 2097152)),
     "gyro_z": AX(B("ABS_RZ"), 1024 * 180 / 3.14, bounds=(-2097152, 2097152)),
 }
 
+MOTION_AXIS_MAP_FLIP_Z: dict[Axis, AX] = {
+    "accel_x": AX(B("ABS_X"), 8192 / 9.8, bounds=(-32768, 32768)),
+    "accel_y": AX(B("ABS_Y"), 8192 / 9.8, bounds=(-32768, 32768)),
+    "accel_z": AX(B("ABS_Z"), 8192 / 9.8, bounds=(-32768, 32768)),
+    "gyro_x": AX(B("ABS_RX"), 1024 * 180 / 3.14, bounds=(-2097152, 2097152)),
+    "gyro_y": AX(B("ABS_RY"), 1024 * 180 / 3.14, bounds=(-2097152, 2097152)),
+    "gyro_z": AX(B("ABS_RZ"), -1024 * 180 / 3.14, bounds=(-2097152, 2097152)),
+}
+
 MOTION_LEFT_AXIS_MAP: dict[Axis, AX] = {
     "left_" + k: v for k, v in MOTION_AXIS_MAP.items()  # type: ignore
 }
 
 MOTION_RIGHT_AXIS_MAP: dict[Axis, AX] = {
     "right_" + k: v for k, v in MOTION_AXIS_MAP.items()  # type: ignore
 }
```

### Comparing `hhd-2.6.5/src/hhd/device/generic/__init__.py` & `hhd-2.7.0/src/hhd/device/generic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,16 +123,16 @@
         if vendor == "ayn":
             return [GenericControllersPlugin(dmi, get_default_config(dmi, "AYN"))]
     except Exception:
         pass
 
     # Fallback to chassis vendor for aya
     try:
-        with open("/sys/devices/virtual/dmi/id/sys_vendor") as f:
+        with open("/sys/class/dmi/id/board_vendor") as f:
             vendor = f.read().lower().strip()
 
-        if "aya" in vendor:
+        if "ayaneo" in vendor:
             return [GenericControllersPlugin(dmi, get_default_config(dmi, "AYA"))]
     except Exception:
         return []
 
     return []
```

### Comparing `hhd-2.6.5/src/hhd/device/generic/base.py` & `hhd-2.7.0/src/hhd/device/generic/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/generic/const.py` & `hhd-2.7.0/src/hhd/device/generic/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/generic/controllers.yml` & `hhd-2.7.0/src/hhd/device/generic/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/gpd/win/__init__.py` & `hhd-2.7.0/src/hhd/device/gpd/win/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/gpd/win/base.py` & `hhd-2.7.0/src/hhd/device/gpd/win/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/gpd/win/const.py` & `hhd-2.7.0/src/hhd/device/gpd/win/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/gpd/win/controllers.yml` & `hhd-2.7.0/src/hhd/device/gpd/win/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/legion_go/__init__.py` & `hhd-2.7.0/src/hhd/device/legion_go/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/legion_go/base.py` & `hhd-2.7.0/src/hhd/device/legion_go/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import select
 import time
 from threading import Event as TEvent
 from typing import Sequence
 
 from hhd.controller import Axis, Button, Consumer, Event, Producer
 from hhd.controller.base import Multiplexer, TouchpadAction
-from hhd.controller.lib.hid import enumerate_unique
 from hhd.controller.physical.evdev import B as EC
 from hhd.controller.physical.evdev import GenericGamepadEvdev, enumerate_evs
 from hhd.controller.physical.imu import AccelImu, GyroImu
 from hhd.controller.virtual.uinput import (
     HHD_PID_MOTION,
     HHD_PID_VENDOR,
     MOTION_CAPABILITIES,
@@ -355,26 +354,28 @@
         emit=emit,
         imu=simu,
         params=d_params,
     )
 
     d_right = UInputDevice(
         name="Handheld Daemon Controller Right Motion Sensors",
-        phys="phys-hhd-main",
+        phys="phys-hhd-lgo-right",
+        uniq="phys-hhd-lgo-right",
         capabilities=MOTION_CAPABILITIES,
         pid=HHD_PID_MOTION,
         btn_map={},
         axis_map=MOTION_RIGHT_AXIS_MAP,
         output_imu_timestamps="right_imu_ts",
         input_props=MOTION_INPUT_PROPS,
         ignore_cmds=True,
     )
     d_left = UInputDevice(
         name="Handheld Daemon Controller Left Motion Sensors",
-        phys="phys-hhd-main",
+        phys="phys-hhd-lgo-left",
+        uniq="phys-hhd-lgo-left",
         capabilities=MOTION_CAPABILITIES,
         pid=HHD_PID_MOTION,
         btn_map={},
         axis_map=MOTION_LEFT_AXIS_MAP,
         output_imu_timestamps="left_imu_ts",
         input_props=MOTION_INPUT_PROPS,
         ignore_cmds=True,
@@ -504,60 +505,52 @@
         ),
     ):
         self.parent = parent
         self.state = False
 
         self.forward_buttons = forward_buttons
         self.passthrough = passthrough
+        self.pressed_time = None
 
         self.to_disable_btn = set()
         self.to_disable_axis = set()
 
     def open(self) -> Sequence[int]:
         return self.parent.open()
 
     def close(self, exit: bool) -> bool:
         return self.parent.close(exit)
 
     def produce(self, fds: Sequence[int]) -> Sequence[Event]:
         evs: Sequence[Event] = self.parent.produce(fds)
 
         out = []
-        prev_state = self.state
+        curr = time.perf_counter()
+        passthrough = self.pressed_time and (curr - self.pressed_time < 1)
+
         for ev in evs:
-            if ev["type"] == "button" and ev["code"] in self.forward_buttons:
-                self.state = ev.get("value", False)
+            if (
+                ev["type"] == "button"
+                and ev["code"] in self.forward_buttons
+                and ev.get("value", False)
+            ):
+                self.pressed_time = curr
 
             if ev["type"] == "configuration":
                 out.append(ev)
             elif ev["type"] == "button" and ev["code"] in self.passthrough:
                 out.append(ev)
             elif ev["type"] == "axis" and (
                 "imu" in ev["code"] or "accel" in ev["code"] or "gyro" in ev["code"]
             ):
                 out.append(ev)
             elif "touchpad" in ev["code"]:
                 out.append(ev)
-            elif ev["type"] == "button" and self.state:
-                self.to_disable_btn.add(ev["code"])
-            elif ev["type"] == "axis" and self.state:
-                self.to_disable_axis.add(ev["code"])
 
-        if self.state:
+        if passthrough:
             # If mode is pressed, forward all events
             return evs
-        elif prev_state:
-            # If prev_state, meaning the user released the mode or share button
-            # turn off all buttons that were pressed during it
-            for btn in self.to_disable_btn:
-                out.append({"type": "button", "code": btn, "value": False})
-            self.to_disable_btn = set()
-            for axis in self.to_disable_axis:
-                out.append({"type": "axis", "code": axis, "value": 0})
-            self.to_disable_axis = set()
-            return out
         else:
-            # Otherwise, just return the standard buttons
             return out
 
     def consume(self, events: Sequence[Event]):
         return self.parent.consume(events)
```

### Comparing `hhd-2.6.5/src/hhd/device/legion_go/const.py` & `hhd-2.7.0/src/hhd/device/legion_go/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/legion_go/controllers.yml` & `hhd-2.7.0/src/hhd/device/legion_go/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/legion_go/gyro_fix.py` & `hhd-2.7.0/src/hhd/device/legion_go/gyro_fix.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/legion_go/hid.py` & `hhd-2.7.0/src/hhd/device/legion_go/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/orange_pi/__init__.py` & `hhd-2.7.0/src/hhd/device/orange_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/orange_pi/base.py` & `hhd-2.7.0/src/hhd/device/orange_pi/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,23 +110,23 @@
         # postprocess=DINPUT_AXIS_POSTPROCESS,
     )
 
     d_kbd_1 = GenericGamepadEvdev(
         vid=[KBD_VID],
         pid=[KBD_PID],
         required=False,
-        # grab=True,
+        grab=False,
         btn_map=dconf.get("at_mapping", AT_BTN_MAPPINGS),
     )
 
     d_kbd_2 = GenericGamepadEvdev(
         vid=GAMEPAD_VIDS,
         pid=GAMEPAD_PIDS,
         required=False,
-        # grab=True,
+        grab=False,
         capabilities={EC("EV_KEY"): [EC("KEY_F16")]},
         btn_map=dconf.get("gamepad_mapping", GAMEPAD_BTN_MAPPINGS),
     )
 
     multiplexer = Multiplexer(
         trigger="analog_to_discrete",
         dpad="analog_to_discrete",
```

### Comparing `hhd-2.6.5/src/hhd/device/orange_pi/const.py` & `hhd-2.7.0/src/hhd/device/orange_pi/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/orange_pi/controllers.yml` & `hhd-2.7.0/src/hhd/device/orange_pi/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/rog_ally/__init__.py` & `hhd-2.7.0/src/hhd/device/rog_ally/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/rog_ally/base.py` & `hhd-2.7.0/src/hhd/device/rog_ally/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/rog_ally/const.py` & `hhd-2.7.0/src/hhd/device/rog_ally/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/rog_ally/controllers.yml` & `hhd-2.7.0/src/hhd/device/rog_ally/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/device/rog_ally/hid.py` & `hhd-2.7.0/src/hhd/device/rog_ally/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/http/api.py` & `hhd-2.7.0/src/hhd/http/api.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/http/i18n.py` & `hhd-2.7.0/src/hhd/http/i18n.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/http/index.html` & `hhd-2.7.0/src/hhd/http/index.html`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/http/static/index.js` & `hhd-2.7.0/src/hhd/http/static/index.js`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo` & `hhd-2.7.0/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo` & `hhd-2.7.0/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo` & `hhd-2.7.0/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo` & `hhd-2.7.0/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/logging.py` & `hhd-2.7.0/src/hhd/logging.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/__init__.py` & `hhd-2.7.0/src/hhd/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/conf.py` & `hhd-2.7.0/src/hhd/plugins/conf.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/display/__init__.py` & `hhd-2.7.0/src/hhd/plugins/display/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/gyro.yml` & `hhd-2.7.0/src/hhd/plugins/gyro.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/inputs.py` & `hhd-2.7.0/src/hhd/plugins/inputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/outputs.py` & `hhd-2.7.0/src/hhd/plugins/outputs.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 
 from ..controller.base import Consumer, Producer
 from ..controller.virtual.dualsense import Dualsense, TouchpadCorrectionType
 from ..controller.virtual.uinput import (
     HHD_PID_MOTION,
     HHD_PID_TOUCHPAD,
     MOTION_AXIS_MAP,
+    MOTION_AXIS_MAP_FLIP_Z,
     MOTION_CAPABILITIES,
     MOTION_INPUT_PROPS,
     TOUCHPAD_AXIS_MAP,
     TOUCHPAD_BUTTON_MAP,
     TOUCHPAD_CAPABILITIES,
+    CONTROLLER_THEMES,
     UInputDevice,
 )
 from .plugin import is_steam_gamepad_running
 from .utils import load_relative_yaml
 
 logger = logging.getLogger(__name__)
 
 
 def get_outputs(
     conf, touch_conf, motion: bool = False, *, controller_id: int = 0, emit=None
 ) -> tuple[Sequence[Producer], Sequence[Consumer], Mapping[str, Any]]:
     producers = []
     consumers = []
+    nintendo_qam = False
 
     controller = conf["mode"].to(str)
     desktop_disable = False
     if touch_conf is not None:
         touchpad = touch_conf["mode"].to(str)
         correction = touch_conf["controller.correction"].to(TouchpadCorrectionType)
         if touchpad in ("emulation", "controller"):
@@ -81,29 +84,64 @@
                 paddles_to_clicks=conf["dualsense.paddles_to_clicks"].to(bool),
                 flip_z=conf["dualsense.flip_z"].to(bool),
                 controller_id=controller_id,
             )
             producers.append(d)
             consumers.append(d)
         case "uinput":
-            d = UInputDevice(phys="phys-hhd-main")
+            theme = conf["uinput.theme"].to(str)
+            if theme == "other":
+                theme = conf["uinput.other_themes"].to(str)
+            nintendo_qam = "switch" in theme or "joy" in theme
+            vid, pid, name = CONTROLLER_THEMES[theme]
+            bus = 0x03 if theme == "hhd" else 0x06
+            addr = "phys-hhd-main"
+            if controller_id:
+                addr = f"phys-hhd-{controller_id:02d}"
+            d = UInputDevice(name=name, vid=vid, pid=pid, phys=addr, uniq=addr)
             producers.append(d)
             consumers.append(d)
             if motion:
-                d = UInputDevice(
-                    name="Handheld Daemon Controller Motion Sensors",
-                    phys="phys-hhd-main",
-                    capabilities=MOTION_CAPABILITIES,
-                    pid=HHD_PID_MOTION,
-                    btn_map={},
-                    axis_map=MOTION_AXIS_MAP,
-                    output_imu_timestamps=True,
-                    input_props=MOTION_INPUT_PROPS,
-                    ignore_cmds=True,
-                )
+                if "xbox" in theme:
+                    d = UInputDevice(
+                        name=f"Handheld Daemon Motion Sensors",
+                        pid=HHD_PID_MOTION,
+                        phys="phys-hhd-imu",
+                        uniq="phys-hhd-imu",
+                        bus=0x03,
+                        capabilities=MOTION_CAPABILITIES,
+                        btn_map={},
+                        axis_map=(
+                            MOTION_AXIS_MAP_FLIP_Z
+                            if conf["uinput.flip_z"].to(bool)
+                            else MOTION_AXIS_MAP
+                        ),
+                        output_imu_timestamps=True,
+                        input_props=MOTION_INPUT_PROPS,
+                        ignore_cmds=True,
+                    )
+                else:
+                    d = UInputDevice(
+                        name=f"{name} Motion Sensors",
+                        vid=vid,
+                        pid=pid,
+                        phys=addr,
+                        uniq=addr,
+                        bus=bus,
+                        capabilities=MOTION_CAPABILITIES,
+                        btn_map={},
+                        axis_map=(
+                            MOTION_AXIS_MAP_FLIP_Z
+                            if conf["uinput.flip_z"].to(bool)
+                            else MOTION_AXIS_MAP
+                        ),
+                        output_imu_timestamps=True,
+                        input_props=MOTION_INPUT_PROPS,
+                        ignore_cmds=True,
+                    )
                 producers.append(d)
                 consumers.append(d)
         case _:
             raise RuntimeError(f"Invalid controller type: '{controller}'.")
 
     if touchpad == "emulation" and steam_check is not False:
         d = UInputDevice(
@@ -125,14 +163,15 @@
         consumers,
         {
             "uses_touch": uses_touch,
             "uses_leds": uses_leds,
             "is_dual": False,
             "steam_check": steam_check,
             "steam_check_fn": lambda: emit and is_steam_gamepad_running(emit.ctx),
+            "nintendo_qam": nintendo_qam,
         },
     )
 
 
 def get_outputs_config(
     can_disable: bool = False,
     has_leds: bool = True,
```

### Comparing `hhd-2.6.5/src/hhd/plugins/outputs.yml` & `hhd-2.7.0/src/hhd/plugins/outputs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,58 @@
     tags: [lgc_emulation_uinput, uinput]
     title: Xbox
     hint: >-
       Creates a virtual `Handheld Daemon Controller` that can be used normally
       in apps. Back buttons are supported but steam will not detect them.
       If Gyroscope or Accelerometer are enabled, a Motion device will be
       created as well (experimental; works in Dolphin).
+    children:
+      theme:
+        type: multiple
+        title: Controller Theme [ALPHA]
+        hint: >-
+          Changes how the controller appears to the System and Steam. Changes the
+          VID/PID of the controller to match the IsJoystick SDL cases.
+          You need to configure the variable `SDL_GAMECONTROLLERCONFIG` for the 
+          extra buttons to work (or use Steam's Setup Input).
+        default: hhd
+        options:
+          hhd: Handheld Daemon
+          xbox_one_elite: Xbox Elite (Paddles)
+          joycon_pair: Joycon Pair (Gyro, Paddles)
+          switch_pro: Switch Pro (Gyro)
+          xbox_360: Xbox 360 (Compatibility)
+          other: Other [ADVANCED]
+      other_themes:
+        type: multiple
+        title: Other Themes
+        default: xbox_one
+        tags: [advanced, expert]
+        options:
+          ps3: DualShock 3
+          ps4: DualShock 4
+          ps5: DualSense
+          ps5e: Dualsense Edge
+          xbox_one: Xbox One
+          xbox_sx: Xbox Series X
+          joycon_left: Joycon Left
+          joycon_right: Joycon Right
+          joycon_grip: Joycon Grip
+          # steam_deck: Steam Deck
+          # steam_controller: Steam Controller
+          steam_input: Steam Virtual Gamepad
+      flip_z:
+        type: bool
+        title: Invert Roll Axis
+        tags: [non-essential]
+        default: True
+        hint: >-
+          Inverts the roll (Z) axis compared to a real Dualsense controller.
+          Useful for Steam Input, since you want it to be inverted to look
+          left to right, but an issue in emulators.
   #
   # Dual Sense 5
   #
   dualsense:
     type: container
     tags: [lgc_emulation_dualsense, dualsense, non-essential]
     title: Dualsense
```

### Comparing `hhd-2.6.5/src/hhd/plugins/overlay/__init__.py` & `hhd-2.7.0/src/hhd/plugins/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/overlay/base.py` & `hhd-2.7.0/src/hhd/plugins/overlay/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/overlay/controllers.py` & `hhd-2.7.0/src/hhd/plugins/overlay/controllers.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/overlay/overlay.py` & `hhd-2.7.0/src/hhd/plugins/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/overlay/x11.py` & `hhd-2.7.0/src/hhd/plugins/overlay/x11.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/plugin.py` & `hhd-2.7.0/src/hhd/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/powerbutton/__init__.py` & `hhd-2.7.0/src/hhd/plugins/powerbutton/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/powerbutton/base.py` & `hhd-2.7.0/src/hhd/plugins/powerbutton/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/powerbutton/const.py` & `hhd-2.7.0/src/hhd/plugins/powerbutton/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,43 +22,44 @@
     PBC("ROG Ally", "ROG Ally RC71L_RC71L"),
     PBC("ROG Ally", "ROG Ally RC71L"),
     PBC("GPT Win 4", "G1618-04"),
     PBC("GPD Win Mini", "G1617-01"),
     PBC("GPD Win Max 2 2023", "G1619-05"),
     PBC("OrangePi G1621-02/G1621-02", "G1621-02"),
     PBC("OrangePi NEO-01/NEO-01", "NEO-01"),
-    PBC(
-        "Steam Deck LCD",
-        "Jupiter",
-        type="hold_emitted",
-        phys=["isa0060", "PNP0C0C", "LNXPWRBN"],
-    ),
-    PBC(
-        "Steam Deck OLED",
-        "Galileo",
-        type="hold_emitted",
-        phys=["isa0060", "PNP0C0C", "LNXPWRBN"],
-    ),
+    # breaks volume buttons, use the valve original script and hope steam inhibits systemd
+    # PBC(
+    #     "Steam Deck LCD",
+    #     "Jupiter",
+    #     type="hold_emitted",
+    #     phys=["isa0060", "PNP0C0C", "LNXPWRBN"],
+    # ),
+    # PBC(
+    #     "Steam Deck OLED",
+    #     "Galileo",
+    #     type="hold_emitted",
+    #     phys=["isa0060", "PNP0C0C", "LNXPWRBN"],
+    # ),
     PBC(
         "AOKZOE A1",
         "AOKZOE A1 AR07",
         type="hold_emitted",
-        phys=["LNXPWRBN"],
+        phys=["LNXPWRBN", "PNP0C0C"],
     ),
     PBC(
         "AOKZOE A1 Pro",
         "AOKZOE A1 Pro",
         type="hold_emitted",
-        phys=["LNXPWRBN"],
+        phys=["LNXPWRBN", "PNP0C0C"],
     ),
     PBC(
         "ONEXPLAYER Mini Pro",
         "ONEXPLAYER Mini Pro",
         type="hold_emitted",
-        phys=["LNXPWRBN"],
+        phys=["LNXPWRBN", "PNP0C0C"],
     ),
 ]
 
 
 def get_config() -> PowerButtonConfig:
     with open("/sys/devices/virtual/dmi/id/product_name") as f:
         prod = f.read().strip()
```

### Comparing `hhd-2.6.5/src/hhd/plugins/settings.py` & `hhd-2.7.0/src/hhd/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/touchpad.yml` & `hhd-2.7.0/src/hhd/plugins/touchpad.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/plugins/utils.py` & `hhd-2.7.0/src/hhd/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/settings.yml` & `hhd-2.7.0/src/hhd/settings.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd/utils.py` & `hhd-2.7.0/src/hhd/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/src/hhd.egg-info/PKG-INFO` & `hhd-2.7.0/src/hhd.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.6.5
+Version: 2.7.0
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -33,291 +33,180 @@
 <!-- [![]()]() -->
 
 # Handheld Daemon
 Handheld Daemon is a project that aims to provide utilities for managing handheld
 devices.
 It features a fully functional controller emulator that exposes gyro,
 paddles, LEDs and QAM across Steam, RPCS3, Dolphin and others.
-In addition, it features TDP controls for Ryzen devices (beta) and manufacturer
-TDP controls for the Legion Go.
+In addition, it features TDP controls all Ryzen devices and bespoke manufacturer
+controls for the Legion Go and ROG Ally.
 It brings all supported devices up to parity with Steam Deck.
 Read [supported devices](#supported-devices) to see if your device is supported.
 
-Handheld Daemon exposes configuration through an API, and there is already a Decky
-plugin for it ([hhd-decky](https://github.com/hhd-dev/hhd-decky)) and a steam
-overlay, web app for it ([hhd.dev](https://hhd.dev)) that also works locally with Electron
+Handheld Daemon exposes configuration through an API, with a gamemode overlay
+(double press/hold Side Menu), Decky plugin ([hhd-decky](https://github.com/hhd-dev/hhd-decky)),
+web app ([hhd.dev](https://hhd.dev)) and desktop app
 ([hhd-ui](https://github.com/hhd-dev/hhd-ui)).
 
 *Current Features*:
-- Fully functional DualSense and Dualsense Edge emulation
-    - All buttons supported
-    - Rumble feedback
-    - Touchpad support (Steam Input as well)
-    - LED remapping
-- Xbox 360 Style device emulation
+- DualSense and Dualsense Edge emulation
+  - All buttons supported
+  - Rumble feedback
+  - Touchpad support (Steam Input as well)
+  - LED remapping
+- Xbox Elite emulation
   - No weird glyphs
-  - Gyro and back button support (outside Steam)
+  - Back button support
+- Complete SDL UInput Emulation
+  - Joycon (Left, Right, Pair), Switch Pro, Dualsense (Edge), Xbox One, Xbox Series X, Xbox 360
+  - Gyro + Paddles for all SDL apps 
   - Dual Evdev Motion Controllers for Legion Go
 - Virtual Touchpad Emulation
-  - Fixes left and right clicks within gamescope when using the device touchpad.
+  - Fixes left and right clicks within gamemode when using the device touchpad.
 - Power Button plugin for Big Picture/Steam Deck Mode
   - Short press makes Steam backup saves and wink before suspend.
   - Long press opens Steam power menu.
 - TDP Controls ([adjustor](https://github.com/hhd-dev/adjustor))
-- Fully Featured Steam Overlay
-- UI based Configuration
-  - Generic API that can be used from bash scripts (through `curl`)
-  - Decky Plugin
-  - Gamemode Overlay, web app, and desktop app
+  - For ROG Ally and Legion Go: 
+    - TDP, Fan Curves, Charge Limiting the Asus and Lenovo way
+    - Asus: Kernel Driver
+    - Lenovo: acpi_call while the kernel driver is being developed
+  - For Other Devices without firmware TDP controls:
+    - acpi_call + AMD's official manufacturer TDP ACPI bindings
+    - Ayaneo, Ayn, GPD, OneXPlayer
+- Configuration:
+  - Fully Featured Gamemode (Gamescope) Overlay
+  - Desktop App
+  - Web app
+  - Config files
 - Built-in updater.
 
 ## Showcase
 ![Overlay](./docs/overlay.gif)
 
 ## <a name="devices"></a>Supported Devices
-The following devices have been verified to work correctly, with QAM, 
+The following devices have been verified to work correctly, with TDP, QAM, 
 Paddles/extra buttons, RGB remapping, Touchpad, and Gyro support.
 The gyro axis might be incorrect for some of those devices, and can be easily
 fixed in the configuration menu by following [these steps](#axis).
 If you do take the time, please open an issue with the correct mapping so it
 is added to your device.
 
 - Legion Go
 - ROG Ally
 - GPD Win 
-  - Win 4
+  - Win 4 (No LEDs)
   - Win Mini
   - Win Max 2 2023
 - Ayaneo
   - Air Standard/Plus/Pro
   - 1S/1S Limited
   - 2/2S 
   - GEEK, GEEK 1S 
   - NEXT Lite/Pro/Advance
   - SLIDE
+  - 2021 Standard/Pro/Pro Retro Power
+  - NEO 2021/Founder
 - Ayn
   - Loki Zero/Max
 - AOKZOE
-  - A1
-  - A1 Pro 
+  - A1 Normal/Pro (No LEDs)
 - Onexplayer
   - Mini Pro
 
 In addition, Handheld Daemon will attempt to work on Ayaneo, Ayn, Onexplayer, and 
 GPD Win devices that have not been verified to work 
 (controller emulation will be off on first start).
 If everything works and you fix the gyro axis for your device, open an issue
 so that your device can be added to the supported list.
 The touchpad will not work for devices not on the supported list.
 
-RGB support is not yet available for GPD Win 4, it is currently being investigated.
-In addition, GPD Win 4's touch point acts like a mouse, so it unfortunately can not
-be used for steam input.
-Some devices do not support holding the power button to open steam settings on
-the current version, this will be fixed in a future release.
-
 ## Installation Instructions
-You can install the latest stable version of `hhd` from PyPi (recommended), AUR,
-or COPR.
-The easiest way to use Handheld Daemon is to install Bazzite which
-comes pre-installed with the latest version and all required kernel
-fixes for supported devices, see [here](#bazzite).
-Nobara also packages hhd and it will become the default for supported devices soon.
-However, it only packages fixes for the Ally and Legion Go at the time of this
-writing.
-
-> [!IMPORTANT]
-> To ensure the gyro of the Legion Go with AMD SFH runs smoothly, 
-> a udev rule is included that disables the use of the accelerometer by the 
-> system (e.g., iio-sensor-proxy).
-> If you want display auto rotation to work, see manual local steps.
-
-### Automatic Local Install
-You can use the following bash scripts to install and uninstall Handheld Daemon.
-Then, update from Decky or the UI.
-These steps do not work on Bazzite, see [here](#bazzite).
-
+Use the following script to install Handheld Daemon or find your OS [here](#os-install):
 ```bash
-# Install
 curl -L https://github.com/hhd-dev/hhd/raw/master/install.sh | sh
-
-# Uninstall
-curl -L https://github.com/hhd-dev/hhd/raw/master/uninstall.sh | sh
-```
-
-You can also install the Decky plugin.
-Having Decky installed is a prerequisite ([instructions](https://github.com/SteamDeckHomebrew/decky-loader#-installation)).
-```bash
-curl -L https://github.com/hhd-dev/hhd-decky/raw/main/install.sh | sh
 ```
 
-Then, reboot and go to [hhd.dev](https://hhd.dev) to configure or read more in
-the [configuration section](#configuration).
+You can use this script on NobaraOS (after uninstalling the built-in Handheld Daemon/HandyGCCS).
+ChimeraOS up to 45-1 is not supported due to general instability (uninstall HandyGCCS if you do).
+This does not work and is not needed on Bazzite, see [here](#bazzite).
+
+> [!IMPORTANT]  
+> For non-gaming distros, see [here](./kernel.md) for a partial list of kernel 
+> patches. This includes `acpi_call` for TDP on devices other than the Ally.
 
-> [!IMPORTANT]
-> Before creating an issue, make sure you are using the latest Handheld Daemon 
-> version and that you read the extra information for each setting in 
-> either [hhd.dev](https://hhd.dev) or the `state.yml` file.
-> 
-> The context is required to understand what each setting does and is 
-> not included in the current version of the Decky Plugin 
-> due to UI limitations.
-
-#### Using an older version
-If you find any issues with the latest version of Handheld Daemon
-you can use any version by specifying it with the command below.
+You can also install the Decky plugin (optional; decky required):
+([instructions](https://github.com/SteamDeckHomebrew/decky-loader#-installation)):
 ```bash
-sudo systemctl stop hhd_local@$(whoami)
-~/.local/share/hhd/venv/bin/pip install hhd==1.0.6
-sudo systemctl start hhd_local@$(whoami)
+curl -L https://github.com/hhd-dev/hhd-decky/raw/main/install.sh | sh
 ```
 
-### Manual Local Installation
-You can also install Handheld Daemon using a local package, which enables auto-updating.
-These are the same steps as done in the Automatic Install (also see 
-[Common Issues after Install](#issues)).
-These steps do not work on Bazzite, see [here](#bazzite).
-
+### Uninstall
+We are sorry to see you go, use the following to uninstall:
 ```bash
-# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-# !!!! Uninstall HandyGCCS to avoid issues if you have it. !!!!
-# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-
-# Install Handheld Daemon to ~/.local/share/hhd
-mkdir -p ~/.local/share/hhd && cd ~/.local/share/hhd
-
-python3 -m venv --system-site-packages venv
-source venv/bin/activate
-pip install --upgrade hhd adjustor
-# Substitute with the following to pull from github (may not always work)
-# pip install git+https://github.com/hhd-dev/hhd git+https://github.com/hhd-dev/hhd-ui
-
-# Install the UI to ~/.local/bin
-FINAL_URL='https://api.github.com/repos/hhd-dev/hhd-ui/releases/latest'
-curl -L $(curl -s "${FINAL_URL}" | grep "browser_download_url" | cut -d '"' -f 4) -o $HOME/.local/bin/hhd-ui
-chmod +x $HOME/.local/bin/hhd-ui
-
-# Install udev rules and create a service file
-sudo curl https://raw.githubusercontent.com/hhd-dev/hhd/master/usr/lib/udev/rules.d/83-hhd.rules -o /etc/udev/rules.d/83-hhd.rules
-sudo curl https://raw.githubusercontent.com/hhd-dev/hhd/master/usr/lib/udev/hwdb.d/83-hhd.hwdb -o /etc/udev/hwdb.d/83-hhd.hwdb
-sudo curl https://raw.githubusercontent.com/hhd-dev/hhd/master/usr/lib/systemd/system/hhd_local%40.service -o /etc/systemd/system/hhd_local@.service
-
-# Change rules to re-enable display autorotation if you do not want gyro support.
-# sudo nano /etc/udev/rules.d/83-hhd.rules
-
-# Start service and reboot
-sudo systemctl enable hhd_local@$(whoami)
-sudo reboot
+curl -L https://github.com/hhd-dev/hhd/raw/master/uninstall.sh | sh
 ```
 
-#### Using an older version
+### Using an older version
 If you find any issues with the latest version of Handheld Daemon
 you can use any version by specifying it with the command below.
 ```bash
 sudo systemctl stop hhd_local@$(whoami)
-~/.local/share/hhd/venv/bin/pip install hhd==1.0.6
+~/.local/share/hhd/venv/bin/pip install hhd==2.6.0
 sudo systemctl start hhd_local@$(whoami)
 ```
 
-#### Update Instructions
-Of course, you will want to update Handheld Daemon to catch up to latest features.
-You can either use the commands below or press `Update (Stable)` in one of the UIs
-(which runs these commands).
-```bash
-sudo systemctl stop hhd_local@$(whoami)
-~/.local/share/hhd/venv/bin/pip install --upgrade hhd
-sudo systemctl start hhd_local@$(whoami)
-```
-
-#### Uninstall instructions
-To uninstall, simply stop the service and remove the added files.
-```bash
-sudo systemctl disable hhd_local@$(whoami)
-sudo systemctl stop hhd_local@$(whoami)
-
-rm -rf ~/.local/share/hhd
-rm -f ~/.local/bin/hhd-ui
-sudo rm /etc/udev/rules.d/83-hhd.rules
-sudo rm /etc/udev/hwdb.d/83-hhd.hwdb
-sudo rm /etc/systemd/system/hhd_local@.service
-
-# Delete your configuration
-rm -r ~/.config/hhd
-```
-### <a name="gyro"></a>Kernel Patches
-There is an optional kernel patch for the Legion Go that increases the Display
-Gyro accuracy [here](https://github.com/hhd-dev/linux-handheld/blob/master/6.6/0001-amd-sfh-bump-sensitivity.patch).
-
-For LED support, the following modules are required for Ayaneo and Ayn: 
-[ayaneo-platform](https://github.com/ShadowBlip/ayaneo-platform)
-driver, and for Ayn, the [ayn-platform](https://github.com/ShadowBlip/ayn-platform).
-Provided these drivers are installed and are supported by your device,
-LED support will be enabled by default.
-
-### Gyro
-Which kernel patch is required will depend on your device's bosch module.
-For the Bosch 260 IMU, you will need the 
-[bmi260-dkms](https://github.com/hhd-dev/bmi260) driver.
-For the Bosch 160 IMU and certain devices, you will need the following bmi160
-[kernel patch](https://github.com/pastaq/bmi160-aya-neo/blob/main/bmi160_ayaneo.patch).
-Ayaneo Air Plus and Ally use the Bosch 323 and need the patch series from
-this repository: [Ally Nobara Fixes](https://github.com/jlobue10/ALLY_Nobara_fixes). 
-The Legion Go does not need kernel patches.
-
-In addition, for most devices, your kernel config should also 
-enable the modules `SYSFS trigger` with `CONFIG_IIO_SYSFS_TRIGGER` and
-`High resolution timer trigger` with `CONFIG_IIO_HRTIMER_TRIGGER`.
-Both are under `Linux Kernel Configuration ─> Device Drivers ─> Industrial I/O support ─> Triggers - standalone`.
-
 ### <a name="issues"></a>After Install Instructions
 #### Extra steps for ROG Ally
-Without an up-to-date `asus-wmi` kernel driver the usb device of the controller
-does not wake up after sleep so Handheld Daemon stops working.
-This patch is included with Linux kernel 6.7.
 You can hold the ROG Crate button to switch to the ROG Ally's Mouse mode to turn
 the right stick into a mouse.
 
+Combinations with the ROG, Armory Crate buttons is not supported in the Ally,
+you can swap them with start/select for this functionality.
+
 #### Extra steps GPD Win Devices
 In order for the back buttons in GPD Win Devices to work, you need to map the
-back buttons to Left: Printscreen, Right: Pause using Windows.
+back buttons to Left: PrintScreen, Right: Pause using Windows.
 This is the default mapping, so if you never remapped them using Windows you
 will not have to.
 Handheld Daemon automatically handles the interval to enable being able to hold
 the buttons.
 
 Here is how the button settings should look:
 ```
 Left-key: PrtSc + 0ms + NC + 0ms + NC + 0ms + NC
 Right-key: Pausc + 0ms + NC + 0ms + NC + 0ms + NC
 ```
 
-Unfortunately, its not possible to rapid double tap the buttons due to their
+Unfortunately, it is not possible to rapid double tap the buttons due to their
 implementation.
 The R4 button is mapped to Side Menu (QAM) by default.
 
 #### Extra steps for Ayaneo/Ayn/Onexplayer
-You might experience a tiny amount of lag with the Ayaneo LEDs
+You might experience a tiny amount of lag with the Ayaneo LEDs.
 The paddles of the Ayn Loki Max are not remappable as far as we know.
 
 #### Extra steps for Legion Go
-If you are using a kernel older than 6.8 and you are not on a gaming distro
-(ChimeraOS, Nobara, Bazzite), you need the following rule for the controllers
+If you have set any mappings on Legion Space, they will interfere with Handheld
+Daemon.
+You can factory reset the Controllers from the Handheld Daemon settings.
+
+The controller gyros of the Legion Go tend to drift and have noise.
+However, they are excellent after calibration.
+Calibrate them using steam calibration and be patient, as they will fail a lot.
+Depending on their state in rare cases they might not be possible to calibrate.
+
+If you are using a kernel older than 6.8, and you are not on a gaming distro
+(Nobara, Bazzite), you need the following rule for the controllers
 to be recognized.
 ```bash
 # Enable xpad for the Legion Go controllers
 ATTRS{idVendor}=="17ef", ATTRS{idProduct}=="6182", RUN+="/sbin/modprobe xpad" RUN+="/bin/sh -c 'echo 17ef 6182 > /sys/bus/usb/drivers/xpad/new_id'"
 ```
 
-If you have set any mappings on Legion Space, they will interfere with Handheld
-Daemon.
-As of version 2.0.0, you can factory reset the controllers from the Handheld
-Daemon settings, or you
-can partially reset them controllers by holding Legion R + RT + RB, 
-and then Legion L + LT + LB or booting into windows.
-
 #### High Touchpad Sensitivity in Steam Input
 By default, the Dualsense kernel driver exposes the Dualsense trackpad as a normal
 trackpad.
 This means that if you go to use it as steam input, you still get the normal
 trackpad input.
 This leads to double input.
 
@@ -330,183 +219,105 @@
 ACTION=="add|change", KERNEL=="event[0-9]*", ATTRS{name}=="*Wireless Controller Touchpad", ENV{LIBINPUT_IGNORE_DEVICE}="1"
 ```
 
 The package `ds-inhibit` is available in AUR, packaged for Nobara, and enabled
 by default in Bazzite.
 
 #### Playstation Glyphs and Controller Image
-If you do not want playstation glyphs in Steam, you can use https://github.com/frazse/PS5-to-Xbox-glyphs
+If you do not want Playstation glyphs in Steam, you can use 
+https://github.com/frazse/PS5-to-Xbox-glyphs
 as a CSS Loader plugin to switch them to Xbox.
 Then, there are CSS plugins for the Legion Go and Ally controller images in
 https://github.com/frazse/SBP-Legion-Go-Theme and 
 https://github.com/semakusut/SBP-ROG-Ally respectively.
-If you are using Bazzite, you can also find a `ujust` version of the commands in 
-the Bazzite readme.
+If you are using Bazzite, you can also find a `ujust` version of the commands 
+in the Bazzite readme.
 
-#### Missing Python Evdev
-In case you have installation issues, you might be missing the package `python-evdev`.
-You can either install it as part of your distribution (included by Nobara
-and ChimeraOS) or automatically through `pip` with the commands above.
-However, installing this package through `pip` requires `base-devel` on Arch and
-`python-devel` on Nobara.
-```bash
-# Nobara/Fedora
-sudo dnf install python-evdev
-# Arch based distros (included by ChimeraOs)
-sudo pacman -S python-evdev
-
-# OR
-
-# (nobara) Install Python Headers since evdev has no wheels
-# and nobara does not ship them (but arch does)
-sudo dnf install python-devel
-# (Chimera, Arch) In case you dont have gcc.
-sudo pacman -S base-devel
-```
+## <a name="configuration"></a>Configuration
+Open the overlay (double press side button), or open the desktop app (`Handheld Daemon`/`$ hhd-ui`),
+or go to [hhd.dev](https://hhd.dev) and enter your device token (`~/.config/hhd/token`).
+Then just start configuring!
 
-#### Having HandyGCCS Installed
-If your distro ships with HandyGCCS Handheld Daemon will not work, you have to uninstall it.
-```bash
-# ChimeraOS
-sudo frzr-unlock
-sudo systemctl disable --now handycon.service
-sudo pacman -R handygccs-git
-
-# Nobara
-sudo systemctl disable --now handycon.service
-sudo dnf remove handygccs-git # (verify ?)
+You can also use the Decky plugin (needs Decky):
 ```
-
-### <a name="bazzite"></a><a name="after-install"></a>Bazzite
-Handheld Daemon comes pre-installed on Bazzite and updates along-side the system.
-The latest version of Handheld Daemon becomes available at the latest the next
-day after release, and can be managed through the Bazzite updater.
-In addition, Bazzite contains all the required kernel patches for the Handheld Daemon
-supported devices, so it is the recommended distro to use Handheld Daemon with.
-
-After install, you can use `ujust` to install Decky and the Handheld Daemon Decky
-plugin with the commands `ujust setup-decky`, `ujust setup-decky hhd-decky`.
-
-If you need to use a different Handheld Daemon version or a custom one, the 
-install steps do not currently work for Bazzite, but this will be fixed in the future.
-Essentially, a new service file needs to be written for Bazzite that contains the
-correct home path (`/var/home`) and then you can disable the built-in version
-service and use the new one instead.
-
-See [supported devices](#supported-devices) to check the status of your device and 
-[after install](#issues) for specific device quirks.
-
-### ❄️ NixOS
-Ensure your `nixpkgs` is on the `unstable` channel (as of Feb 2024):
-
-```nix
-  inputs = {
-    nixpkgs.url = "github:nixos/nixpkgs/nixos-unstable";
+curl -L https://github.com/hhd-dev/hhd-decky/raw/main/install.sh | sh
 ```
 
-and add this line to your `configuration.nix`:
-```nix
-  services.handheld-daemon.enable = true;
-```
+The configuration files are stored under `~/.config/hhd` with the main one being
+`state.yml`, which can be edited and will hot reload.
 
-### Distribution Installation (not recommended)
+## <a name="os-install"></a> Distribution Install
 You can install Handheld Daemon from [AUR](https://aur.archlinux.org/packages/hhd) 
 (Arch) or [COPR](https://copr.fedorainfracloud.org/coprs/hhd-dev/hhd/) (Fedora).
 Both update automatically every time there is a new release.
 
 But, the auto-updater will not work, which is an important feature with devices
 without a keyboard.
 ```bash
 # Arch
-yay -S hhd hhd-ui adjustor
+yay -S hhd adjustor hhd-ui
 
 # Fedora
 sudo dnf copr enable hhd-dev/hhd
-sudo dnf install hhd adjustor
-# HHD-UI todo
+sudo dnf install hhd adjustor hhd-ui
 
-# Enable and reboot
 sudo systemctl enable hhd@$(whoami)
-sudo reboot
 ```
 
-In case you do not want to reboot.
-```bash
-# Reload Handheld Daemon's udev rules
-sudo udevadm control --reload-rules && sudo udevadm trigger
-# Restart iio-proxy-service to stop it
-# from polling the accelerometer
-sudo systemctl restart iio-sensor-proxy
-# Start the service for your user
-sudo systemctl start hhd@$(whoami)
-```
+### ❄️ NixOS
+Handheld Daemon (core; no overlay, TDP) is on `nixpkgs` in the `unstable` channel.
 
-## <a name="configuration"></a>Configuration
-### UI Based
-Go to [hhd.dev](https://hhd.dev) and enter your device token 
-(`~/.config/hhd/token`).
-That is it!
-You can also install the Electron version ([hhd-ui](https://github.com/hhd-dev/hhd-ui)) 
-to use completely offline or as an app (updating it has to be done manually for now).
-
-### Using Decky
-If you have decky installed, you can use the following command to
-install the Handheld Daemon decky plugin (visit 
-[hhd-decky](https://github.com/hhd-dev/hhd-decky) for details).
-```
-curl -L https://github.com/hhd-dev/hhd-decky/raw/main/install.sh | sh
+Add the following to your `configuration.nix` to enable:
+```nix
+  services.handheld-daemon.enable = true;
+  services.handheld-daemon.user = "<your-user>";
 ```
-Then, just open up steam.
 
-### File based
-The reason you added your username to the `hhd` service was to bind the `hhd`
-daemon to your user.
+### <a name="bazzite"></a><a name="after-install"></a>Bazzite
+Handheld Daemon comes pre-installed on [Bazzite](https://bazzite.gg) and 
+updates along-side the system.
+Most users of Handheld Daemon are on Bazzite and Bazzite releases
+often happen to bundle Handheld Daemon.
+Bazzite contains all kernel patches and quirks required for all supported handhelds
+to work (to the extent they can; certain Ayaneo devices have issues.)
 
-This allows Handheld Daemon to add configuration files with appropriate
-permissions to your user, in the following directory:
-```bash
-~/.config/hhd
-```
+After install, you can use `ujust` to install Decky and the Handheld Daemon Decky
+plugin with the commands `ujust setup-decky`, `ujust setup-decky hhd-decky`.
 
-The global configuration for HHD is found in:
-```bash
-~/.config/hhd/state.yml
-```
+If you need to use a different Handheld Daemon version or a custom one, the 
+install steps do not currently work for Bazzite, a `ujust` command is in the works.
 
-You can modify it and it will hot-reload upon saving.
+See [supported devices](#supported-devices) to check the status of your device and 
+[after install](#issues) for specific device quirks.
 
 ## Contributing
 ### <a name="axis"></a> Finding the correct axis for your device
-To figure the correct axis from your device, go to desktop and open the steam
-calibration settings.
-Then, go to https://hhd.dev , switch `Motion Axis` to `Override` and tweak only
-the axis (without invert) of your device until they match the glyphs in steam.
-
-> [!WARNING]  
-> Do not try to interpret what each axis means. You will get a headache. 
-> Just change them randomly until
-> the glyphs line up with how you move your controller.
-> If you set multiple axis to a single one (e.g., X to Y, and Y to Y),
-> the first option (e.g., X to Y) option will be ignored.
+To figure the correct axis from your device, go to steam calibration settings.
+Then, in the overlay (double press/hold side button) switch `Motion Axis` to 
+`Override` and tweak only the axis (without invert) of your device until they 
+match the glyphs in steam.
 
 Then, jump in a first person game and turn on `Gyro to Mouse` or `Camera`.
-For `Gyro to Mouse`, use `Gyro to Mouse fix` if you get issues with the camera
-jumping around.
-By default, rotating your device like a steering wheel should turn left to right,
+By default (`Yaw`), rotating your device like a steering wheel should turn left 
+to right,
 and rotating it to face down or up should look up or down.
 Fix the invert settings of the axis so that it is intuitive.
 Finally, switch the setting `Gyro Turning Axis` from `Yaw` (rotate like a steering
 wheel) to `Roll` (turn left to right), and fix the remaining axis inversion.
 
 You can now either take a picture of your screen or translate the settings into
 text (e.g., x is k, y is l inverted, z is j) and open an issue.
 The override setting also displays the make and model of your device, which
 are required to add the mappings to Handheld Daemon.
 
 ### Localizing Handheld Daemon
+Handheld Daemon fully supports localization through standard `PO`, `POT` files.
+Contribution instructions in progress!!!
+
+#### For maintainers
 You can find `pot` and `po` files for Handheld Daemon under the `i18n` directory.
 You can clone/download this repository and open the `./i18n` directory.
 Then, just copy the `*.pot` files into `<your_locale>/LC_MESSAGES/*.po`
 and begin translating with your favorite text editor, or by using
 tool such as [Lokalize](https://apps.kde.org/lokalize/).
 
 As far as your locale goes, unless you have a good reason to, skip the territory
```

### Comparing `hhd-2.6.5/src/hhd.egg-info/SOURCES.txt` & `hhd-2.7.0/src/hhd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 src/hhd/controller/virtual/__init__.py
 src/hhd/controller/virtual/dualsense/__init__.py
 src/hhd/controller/virtual/dualsense/const.py
 src/hhd/controller/virtual/sd/__init__.py
 src/hhd/controller/virtual/sd/const.py
 src/hhd/controller/virtual/uinput/__init__.py
 src/hhd/controller/virtual/uinput/const.py
+src/hhd/controller/virtual/uinput/monkey.py
 src/hhd/device/generic/__init__.py
 src/hhd/device/generic/base.py
 src/hhd/device/generic/const.py
 src/hhd/device/generic/controllers.yml
 src/hhd/device/gpd/win/__init__.py
 src/hhd/device/gpd/win/base.py
 src/hhd/device/gpd/win/const.py
```

### Comparing `hhd-2.6.5/usr/lib/udev/hwdb.d/83-hhd.hwdb` & `hhd-2.7.0/usr/lib/udev/hwdb.d/83-hhd.hwdb`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/usr/lib/udev/rules.d/83-hhd-user.rules` & `hhd-2.7.0/usr/lib/udev/rules.d/83-hhd-user.rules`

 * *Files identical despite different names*

### Comparing `hhd-2.6.5/usr/lib/udev/rules.d/83-hhd.rules` & `hhd-2.7.0/usr/lib/udev/rules.d/83-hhd.rules`

 * *Files identical despite different names*

