# Comparing `tmp/aalto-boss-1.9.1.tar.gz` & `tmp/aalto-boss-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aalto-boss-1.9.1.tar", last modified: Fri Feb 16 14:31:07 2024, max compression
+gzip compressed data, was "aalto-boss-1.9.2.tar", last modified: Mon Mar 18 12:06:33 2024, max compression
```

## Comparing `aalto-boss-1.9.1.tar` & `aalto-boss-1.9.2.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.187701 aalto-boss-1.9.1/
--rw-rw-rw-   0 root         (0) root         (0)    11334 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6185 2024-02-16 14:31:07.186701 aalto-boss-1.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4861 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.174701 aalto-boss-1.9.1/aalto_boss.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6185 2024-02-16 14:31:07.000000 aalto-boss-1.9.1/aalto_boss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2024-02-16 14:31:07.000000 aalto-boss-1.9.1/aalto_boss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 14:31:07.000000 aalto-boss-1.9.1/aalto_boss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-02-16 14:31:07.000000 aalto-boss-1.9.1/aalto_boss.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-02-16 14:31:07.000000 aalto-boss-1.9.1/aalto_boss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-02-16 14:31:07.000000 aalto-boss-1.9.1/aalto_boss.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.175701 aalto-boss-1.9.1/boss/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4799 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.177701 aalto-boss-1.9.1/boss/bo/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.180701 aalto-boss-1.9.1/boss/bo/acq/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4663 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5847 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/cost.py
--rw-rw-rw-   0 root         (0) root         (0)     2504 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/ei.py
--rw-rw-rw-   0 root         (0) root         (0)     3005 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/elcb.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/exploit.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/explore.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     6479 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/kb.py
--rw-rw-rw-   0 root         (0) root         (0)     2063 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/lcb.py
--rw-rw-rw-   0 root         (0) root         (0)     5410 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3831 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/mes.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/acq/multi.py
--rw-rw-rw-   0 root         (0) root         (0)    14943 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/bo_main.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/hmc.py
--rw-rw-rw-   0 root         (0) root         (0)     3715 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/initmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     9766 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/kernel_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    34193 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/model.py
--rw-rw-rw-   0 root         (0) root         (0)    20023 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/results.py
--rw-rw-rw-   0 root         (0) root         (0)     5064 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/rstmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     7293 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/bo/userfunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.181701 aalto-boss-1.9.1/boss/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6054 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/io/dump.py
--rw-rw-rw-   0 root         (0) root         (0)     2971 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/io/ioutils.py
--rw-rw-rw-   0 root         (0) root         (0)    14370 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/io/main_output.py
--rw-rw-rw-   0 root         (0) root         (0)     9058 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/io/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7067 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/keywords.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.183701 aalto-boss-1.9.1/boss/mep/
--rw-rw-rw-   0 root         (0) root         (0)      183 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/mep/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2047 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/mep/forest.py
--rw-rw-rw-   0 root         (0) root         (0)     5746 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/mep/mep.py
--rw-rw-rw-   0 root         (0) root         (0)     3781 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/mep/mepmain.py
--rw-rw-rw-   0 root         (0) root         (0)     2724 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/mep/neb.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/mep/node.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/mep/path.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/mep/space.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.184701 aalto-boss-1.9.1/boss/pp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/pp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21357 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/pp/plot.py
--rw-rw-rw-   0 root         (0) root         (0)    19531 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/pp/pp_main.py
--rw-rw-rw-   0 root         (0) root         (0)    14903 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.184701 aalto-boss-1.9.1/boss/testing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/testing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13955 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/testing/benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)    18064 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/testing/testfunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 14:31:07.186701 aalto-boss-1.9.1/boss/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3762 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/utils/arrays.py
--rw-rw-rw-   0 root         (0) root         (0)     3815 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/utils/distributions.py
--rw-rw-rw-   0 root         (0) root         (0)    11037 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/utils/minimization.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/utils/os.py
--rw-rw-rw-   0 root         (0) root         (0)     6686 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/utils/sparselist.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/utils/timer.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/boss/utils/typing.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-16 14:31:07.187701 aalto-boss-1.9.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3249 2024-02-16 14:31:06.000000 aalto-boss-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.445735 aalto-boss-1.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3264 2024-03-18 12:06:33.444735 aalto-boss-1.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1940 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.434735 aalto-boss-1.9.2/aalto_boss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3264 2024-03-18 12:06:33.000000 aalto-boss-1.9.2/aalto_boss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1340 2024-03-18 12:06:33.000000 aalto-boss-1.9.2/aalto_boss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 12:06:33.000000 aalto-boss-1.9.2/aalto_boss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-03-18 12:06:33.000000 aalto-boss-1.9.2/aalto_boss.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-03-18 12:06:33.000000 aalto-boss-1.9.2/aalto_boss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-03-18 12:06:33.000000 aalto-boss-1.9.2/aalto_boss.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.434735 aalto-boss-1.9.2/boss/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4799 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.436735 aalto-boss-1.9.2/boss/bo/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.439735 aalto-boss-1.9.2/boss/bo/acq/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4663 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5847 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/cost.py
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/ei.py
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/elcb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/exploit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/explore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6479 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/kb.py
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/lcb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5410 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3831 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/mes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/acq/multi.py
+-rw-rw-rw-   0 root         (0) root         (0)    14335 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/bo_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     9376 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/convergence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/hmc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/initmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     9766 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/kernel_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    34193 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/model.py
+-rw-rw-rw-   0 root         (0) root         (0)    20023 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/results.py
+-rw-rw-rw-   0 root         (0) root         (0)     5064 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/rstmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7293 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/bo/userfunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.440735 aalto-boss-1.9.2/boss/io/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6054 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/io/dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     2971 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/io/ioutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14491 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/io/main_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     9058 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/io/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7137 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/keywords.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.441735 aalto-boss-1.9.2/boss/mep/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/mep/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2047 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/mep/forest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5746 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/mep/mep.py
+-rw-rw-rw-   0 root         (0) root         (0)     3781 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/mep/mepmain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2724 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/mep/neb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/mep/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/mep/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/mep/space.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.442735 aalto-boss-1.9.2/boss/pp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/pp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21357 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/pp/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19531 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/pp/pp_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    14625 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.442735 aalto-boss-1.9.2/boss/testing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/testing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13955 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/testing/benchmark.py
+-rw-rw-rw-   0 root         (0) root         (0)    18064 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/testing/testfunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 12:06:33.444735 aalto-boss-1.9.2/boss/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3762 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/utils/arrays.py
+-rw-rw-rw-   0 root         (0) root         (0)     3815 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/utils/distributions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11037 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/utils/minimization.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/utils/os.py
+-rw-rw-rw-   0 root         (0) root         (0)     6686 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/utils/sparselist.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/utils/timer.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/boss/utils/typing.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-18 12:06:33.445735 aalto-boss-1.9.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3249 2024-03-18 12:06:32.000000 aalto-boss-1.9.2/setup.py
```

### Comparing `aalto-boss-1.9.1/LICENSE` & `aalto-boss-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/aalto_boss.egg-info/SOURCES.txt` & `aalto-boss-1.9.2/aalto_boss.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 aalto_boss.egg-info/top_level.txt
 boss/__init__.py
 boss/__main__.py
 boss/keywords.py
 boss/settings.py
 boss/bo/__init__.py
 boss/bo/bo_main.py
+boss/bo/convergence.py
 boss/bo/hmc.py
 boss/bo/initmanager.py
 boss/bo/kernel_factory.py
 boss/bo/model.py
 boss/bo/results.py
 boss/bo/rstmanager.py
 boss/bo/userfunc.py
```

### Comparing `aalto-boss-1.9.1/boss/__init__.py` & `aalto-boss-1.9.2/boss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.9.1"
+__version__ = "1.9.2"
 __url__ = "https://gitlab.com/cest-group/boss"
 __description__ = "Bayesian optimization structure search"
 __authors__ = [
     "Ville Parkkinen",
     "Henri Paulamaki",
     "Arttu Tolvanen",
     "Ulpu Remes",
```

### Comparing `aalto-boss-1.9.1/boss/__main__.py` & `aalto-boss-1.9.2/boss/__main__.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/base.py` & `aalto-boss-1.9.2/boss/bo/acq/base.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/cost.py` & `aalto-boss-1.9.2/boss/bo/acq/cost.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/ei.py` & `aalto-boss-1.9.2/boss/bo/acq/ei.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/elcb.py` & `aalto-boss-1.9.2/boss/bo/acq/elcb.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/exploit.py` & `aalto-boss-1.9.2/boss/bo/acq/exploit.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/explore.py` & `aalto-boss-1.9.2/boss/bo/acq/explore.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/factory.py` & `aalto-boss-1.9.2/boss/bo/acq/factory.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/kb.py` & `aalto-boss-1.9.2/boss/bo/acq/kb.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/lcb.py` & `aalto-boss-1.9.2/boss/bo/acq/lcb.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/manager.py` & `aalto-boss-1.9.2/boss/bo/acq/manager.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/mes.py` & `aalto-boss-1.9.2/boss/bo/acq/mes.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/acq/multi.py` & `aalto-boss-1.9.2/boss/bo/acq/multi.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/bo_main.py` & `aalto-boss-1.9.2/boss/bo/bo_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
-from scipy.spatial.distance import euclidean
 
 import boss.io.ioutils as ioutils
 import boss.io.parse as parse
 from boss.bo.acq.factory import select_acq_manager
+from boss.bo.convergence import select_conv_checker
 from boss.bo.initmanager import InitManager
 from boss.bo.kernel_factory import init_kernel, apply_hyper_settings
 from boss.bo.results import BOResults, minimize_model
 from boss.bo.rstmanager import RstManager
 from boss.io.main_output import MainOutput
 from boss.settings import Settings
 from boss.utils.arrays import shape_consistent_XY
@@ -86,14 +86,15 @@
         self.acqfn.model = self.model
         self.acq_manager = select_acq_manager(settings)
 
         Minimization.set_parallel(self.settings["parallel_optims"])
 
         self.results = BOResults(settings=settings)
         self.results.add_defaults()
+        self.conv_checker = select_conv_checker(settings)
         self.itr_curr = 0
         self.cum_cost = 0
 
     def init_model(self, X, Y, params=None):
         """Initializes the GP model."""
         X, Y = shape_consistent_XY(
             X, Y, self.dim, nan_pad=False, ygrad=self.settings["ygrad"]
@@ -275,15 +276,15 @@
                 # 3. Get a new acquisition for the next iteration.
                 X_next = self.acquire()
 
                 # 4. Update results and write a summary to the outfile.
                 self._update_results(X_next)
 
             # 5. Convergence check
-            if self.has_converged():
+            if self.conv_checker is not None and self.conv_checker(self.results):
                 self.main_output.convergence_stop()
                 break
 
         return self.results
 
     def acquire(self):
         """Gets the next acquisition."""
@@ -379,30 +380,7 @@
         Checks whether the next acquisition would exceed cost limit.
         """
         if self.settings["maxcost"] is None:
             return False
         else:
             cost_next = self.acqfn.evaluate_cost(X_next)
             return self.cum_cost + cost_next > self.settings["maxcost"]
-
-    def has_converged(self):
-        """
-        Checks whether dxhat has been within tolerance for long enough
-        TODO: should use dxmuhat instead?
-        """
-        glmin_tol = self.settings["glmin_tol"]
-        if glmin_tol is None:
-            return False
-
-        conv_tol, conv_itrs = glmin_tol
-        minfreq = self.settings["minfreq"]
-        num_lookback = max(minfreq, conv_itrs) // minfreq
-        x_glmin = self.results["x_glmin"]
-        if len(x_glmin.data) < num_lookback:
-            return False
-
-        for i in range(1, num_lookback + 1):
-            dx = euclidean(x_glmin.value(-i), x_glmin.value(-i - 1))
-            if dx > conv_tol:
-                return False
-
-        return True
```

### Comparing `aalto-boss-1.9.1/boss/bo/hmc.py` & `aalto-boss-1.9.2/boss/bo/hmc.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/initmanager.py` & `aalto-boss-1.9.2/boss/bo/initmanager.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/kernel_factory.py` & `aalto-boss-1.9.2/boss/bo/kernel_factory.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/model.py` & `aalto-boss-1.9.2/boss/bo/model.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/results.py` & `aalto-boss-1.9.2/boss/bo/results.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/rstmanager.py` & `aalto-boss-1.9.2/boss/bo/rstmanager.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/bo/userfunc.py` & `aalto-boss-1.9.2/boss/bo/userfunc.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/io/dump.py` & `aalto-boss-1.9.2/boss/io/dump.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/io/ioutils.py` & `aalto-boss-1.9.2/boss/io/ioutils.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/io/main_output.py` & `aalto-boss-1.9.2/boss/io/main_output.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,21 +132,21 @@
         if not settings.is_rst:
             s += "inittype       %s\n" % (settings["inittype"])
         s += "initpts   %i    iterpts   %i\n" % (
             settings["initpts"],
             settings["iterpts"],
         )
 
-        if settings["glmin_tol"] is not None:
-            s += "glmin_tol         %8.3E   %i\n" % (
-                settings["glmin_tol"][0],
-                settings["glmin_tol"][1],
-            )
+        if settings["convtype"] is not None:
+            s += f"convtype         {settings['convtype']}\n"
+            s += f"conv_reltol         {settings['conv_reltol']:8.3e}\n"
+            s += f"conv_abstol         {settings['conv_reltol']:8.3e}\n"
+            s += f"conv_iters         {settings['conv_reltol']}\n"
         else:
-            s += "glmin_tol         none\n"
+            s += "convtype         none\n"
 
         s += "\n|| Data acquisition \n"
         s += "acqfn                %s\n" % (settings["acqfn_name"])
         s += "acqtol               "
         if settings["acqtol"] is None:
             s += "none\n"
         else:
```

### Comparing `aalto-boss-1.9.1/boss/io/parse.py` & `aalto-boss-1.9.2/boss/io/parse.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/keywords.py` & `aalto-boss-1.9.2/boss/keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,32 +53,34 @@
     "hmciters": 0,
     "minfreq": 1,
     "seed": None,
     "parallel_optims": 0,
     "num_tasks": None,
     "W_rank": 1,
     "batchpts": 1,
+    "conv_iters": 5,
 }
 categories[(int, 1)] = {
     "task_initpts": None,
     "pp_iters": None,
     "pp_model_slice": None,
 }
 categories[(float, 0)] = {
     "noise": 1e-12,
     "acqtol": 0.001,
     "minzacc": 1.0,
     "min_dist_acqs": None,
     "maxcost": None,
     "mep_maxe": None,
     "pp_local_minima": None,
+    "conv_reltol": None,
+    "conv_abstol": 1e-7,
 }
 categories[(float, 1)] = {
     "yrange": None,
-    "glmin_tol": None,
     "periods": None,
     "acqfnpars": np.array([]),
     "task_cost": None,
     "pp_var_defaults": None,
     "thetainit": None,
     "W_init": None,
     "kappa_init": None,
@@ -100,14 +102,15 @@
     "optimtype": "score",
     "thetaprior": "gamma",
     "W_prior": None,
     "kappa_prior": None,
     "costfn": None,
     "costtype": "divide",
     "batchtype": "sequential",
+    "convtype": None,
 }
 categories[(str, 1)] = {
     "userfn": None,
     "kernel": ["rbf"],
 }
 categories[(str, 2)] = {
     "userfn_list": None,
```

### Comparing `aalto-boss-1.9.1/boss/mep/forest.py` & `aalto-boss-1.9.2/boss/mep/forest.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/mep/mep.py` & `aalto-boss-1.9.2/boss/mep/mep.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/mep/mepmain.py` & `aalto-boss-1.9.2/boss/mep/mepmain.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/mep/neb.py` & `aalto-boss-1.9.2/boss/mep/neb.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/mep/node.py` & `aalto-boss-1.9.2/boss/mep/node.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/mep/path.py` & `aalto-boss-1.9.2/boss/mep/path.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/mep/space.py` & `aalto-boss-1.9.2/boss/mep/space.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/pp/plot.py` & `aalto-boss-1.9.2/boss/pp/plot.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/pp/pp_main.py` & `aalto-boss-1.9.2/boss/pp/pp_main.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/settings.py` & `aalto-boss-1.9.2/boss/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,20 +273,14 @@
         kernel = self["kernel"]
         if isinstance(kernel, str):
             self["kernel"] = [kernel]
 
         if len(self["kernel"]) == 1:
             self["kernel"] *= self.dim
 
-        # Exception to the above rule: glmin_tol is a mixed list [float, int]
-        # TODO: break glmin_tol into two keywords in a future release
-        glmin_tol = self["glmin_tol"]
-        if glmin_tol is not None:
-            self["glmin_tol"] = [float(glmin_tol[0]), int(glmin_tol[1])]
-
     def check_acqfn(self):
         """Check the selected acquisition function."""
         if self["maxcost"] is not None:
             if not isinstance(self.acqfn, CostAwareAcquisition):
                 raise ValueError(
                     "A cost-aware acquisition function is needed with the "
                     "keyword 'maxcost'."
@@ -344,16 +338,16 @@
                     "The maximum cost is too low to accommodate for the "
                     "requested initialization data."
                 )
 
     def deprecation_notice(self):
         deprecated = {
             "pp_truef_at_xhats": "pp_truef_at_glmins",
-            "gm_tol": "glmin_tol",
             "verbosity": None,
+            "glmin_tol": "conv_tol and conv_iters"
         }
         msg = ""
         for key, val in deprecated.items():
             if key in self:
                 if val is None:
                     msg += f"Keyword {key} has been deprecated and should be removed\n"
                 else:
```

### Comparing `aalto-boss-1.9.1/boss/testing/benchmark.py` & `aalto-boss-1.9.2/boss/testing/benchmark.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/testing/testfunc.py` & `aalto-boss-1.9.2/boss/testing/testfunc.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/utils/arrays.py` & `aalto-boss-1.9.2/boss/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/utils/distributions.py` & `aalto-boss-1.9.2/boss/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/utils/minimization.py` & `aalto-boss-1.9.2/boss/utils/minimization.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/utils/os.py` & `aalto-boss-1.9.2/boss/utils/os.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/utils/sparselist.py` & `aalto-boss-1.9.2/boss/utils/sparselist.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/boss/utils/timer.py` & `aalto-boss-1.9.2/boss/utils/timer.py`

 * *Files identical despite different names*

### Comparing `aalto-boss-1.9.1/setup.py` & `aalto-boss-1.9.2/setup.py`

 * *Files identical despite different names*

