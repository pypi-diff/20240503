# Comparing `tmp/pytao-0.2.5.tar.gz` & `tmp/pytao-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pytao/pytao/dist/.tmp-ybogoc5a/pytao-0.2.5.tar", last modified: Thu Jul 27 18:45:07 2023, max compression
+gzip compressed data, was "/home/runner/work/pytao/pytao/dist/.tmp-5rbgcfa2/pytao-0.2.6.tar", last modified: Fri May  3 18:15:45 2024, max compression
```

## Comparing `pytao-0.2.5.tar` & `pytao-0.2.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 18:44:56.000000 pytao-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 18:44:56.000000 pytao-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-27 18:45:07.000000 pytao-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-27 18:44:56.000000 pytao-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/data_type_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    34616 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/module_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_base_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_beam_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    50559 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_data_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_ele_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    62214 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_lat_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_misc_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_mpl_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_plot_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    95292 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_plot_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    40433 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_var_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    65690 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/taoplot.py
--rw-r--r--   0 runner    (1001) docker     (123)   114650 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/interface_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/misc/csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/misc/csr_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/misc/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/tao_ctypes/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/extra_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/tao_pexpect/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_pexpect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_pexpect/tao_pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    28283 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tests/test_interface_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/util/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/evaluate_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/lattice_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 18:44:56.000000 pytao-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-27 18:45:07.000000 pytao-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-27 18:44:56.000000 pytao-0.2.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-07-27 18:44:56.000000 pytao-0.2.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:45.000000 pytao-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-03 18:15:35.000000 pytao-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 18:15:35.000000 pytao-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-03 18:15:45.000000 pytao-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-03 18:15:35.000000 pytao-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/data_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34616 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/module_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63664 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_base_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_beam_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10752 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50559 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_data_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_ele_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62214 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_lat_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_misc_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_mpl_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_plot_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95292 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_plot_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40433 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_var_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/tao_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65690 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/gui/taoplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114650 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/interface_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/misc/csr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/misc/csr_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/misc/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao/tao_ctypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tao_ctypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17716 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tao_ctypes/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tao_ctypes/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tao_ctypes/extra_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tao_ctypes/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tao_ctypes/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tao_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao/tao_pexpect/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tao_pexpect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tao_pexpect/tao_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28283 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/tests/test_interface_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/util/evaluate_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/util/lattice_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/util/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-03 18:15:35.000000 pytao-0.2.6/pytao/util/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 18:15:45.000000 pytao-0.2.6/pytao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 18:15:35.000000 pytao-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-03 18:15:45.000000 pytao-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-03 18:15:35.000000 pytao-0.2.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-05-03 18:15:35.000000 pytao-0.2.6/versioneer.py
```

### Comparing `pytao-0.2.5/LICENSE` & `pytao-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/PKG-INFO` & `pytao-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytao
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://www.classe.cornell.edu/bmad/tao.html
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTao
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytao Version: 0.2.5 Home-page: https://
+Metadata-Version: 2.1 Name: pytao Version: 0.2.6 Home-page: https://
 www.classe.cornell.edu/bmad/tao.html Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE # PyTao [PyTao]((https://
 bmad-sim.github.io/pytao/index.html)) is Python interface for [Tao](https://
 www.classe.cornell.edu/bmad/tao.html), which is based on the Bmad subroutine
 library for relativistic chargedâparticle and X-ray simulations in
 accelerators and storage rings. Documentation for Bmad and Tao, as well as
 information for downloading the code if needed is given on the [Bmad website]
```

### Comparing `pytao-0.2.5/README.md` & `pytao-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/__init__.py` & `pytao-0.2.6/pytao/__init__.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/__init__.py` & `pytao-0.2.6/pytao/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/data_type_list.py` & `pytao-0.2.6/pytao/gui/data_type_list.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/main.py` & `pytao-0.2.6/pytao/gui/main.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/module_check.py` & `pytao-0.2.6/pytao/gui/module_check.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_base_windows.py` & `pytao-0.2.6/pytao/gui/tao_base_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_beam_windows.py` & `pytao-0.2.6/pytao/gui/tao_beam_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_console.py` & `pytao-0.2.6/pytao/gui/tao_console.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_data_windows.py` & `pytao-0.2.6/pytao/gui/tao_data_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_ele_location.py` & `pytao-0.2.6/pytao/gui/tao_ele_location.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_interface.py` & `pytao-0.2.6/pytao/gui/tao_interface.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_lat_windows.py` & `pytao-0.2.6/pytao/gui/tao_lat_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_misc_windows.py` & `pytao-0.2.6/pytao/gui/tao_misc_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_mpl_toolbar.py` & `pytao-0.2.6/pytao/gui/tao_mpl_toolbar.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_plot_dict.py` & `pytao-0.2.6/pytao/gui/tao_plot_dict.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_plot_windows.py` & `pytao-0.2.6/pytao/gui/tao_plot_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_set.py` & `pytao-0.2.6/pytao/gui/tao_set.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_var_windows.py` & `pytao-0.2.6/pytao/gui/tao_var_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/tao_widget.py` & `pytao-0.2.6/pytao/gui/tao_widget.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/gui/taoplot.py` & `pytao-0.2.6/pytao/gui/taoplot.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/interface_commands.py` & `pytao-0.2.6/pytao/interface_commands.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/misc/csr.py` & `pytao-0.2.6/pytao/misc/csr.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/misc/csr_plot.py` & `pytao-0.2.6/pytao/misc/csr_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,20 @@
     nsteps = len(data['z'])
     
     stats = np.array([csr_wake_stats_at_step(data, step=i) for i in range(nsteps)])
     print(stats.shape)
     
     fig, ax = plt.subplots(**kwargs)
     
-    ax.set_xlabel('s (m)')
+    ax.set_xlabel(r'$s$ (m)')
     ax.set_ylabel('CSR Kick/m')
     ax.plot(s_pos, stats[:,0], color='black', label='Average Wake')
     ax.plot(s_pos, stats[:,1], color='red', label='std Wake')
     
     ax2 = ax.twinx()
-    ax2.plot(s_pos, stats[:,3]*1e15/299792458, color='blue', label='$\sigma_z/c (fs)$')
-    ax2.set_ylabel('$\sigma_z/c (fs)$')
+    ax2.plot(s_pos, stats[:,3]*1e15/299792458, color='blue', label=r'$\sigma_z/c$ (fs)')
+    ax2.set_ylabel(r'$\sigma_z/c$ (fs)')
     ax.legend()
```

### Comparing `pytao-0.2.5/pytao/misc/markers.py` & `pytao-0.2.6/pytao/misc/markers.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/tao_ctypes/core.py` & `pytao-0.2.6/pytao/tao_ctypes/core.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/tao_ctypes/evaluate.py` & `pytao-0.2.6/pytao/tao_ctypes/evaluate.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         
             g = h5.create_group('expressions')
             for k, v in output.items():
                 if v:
                     g.attrs[k] = v
                     
             # CSR wake
-            csr_wake_file = os.path.join(M.path, 'csr_wake.dat')
+            csr_wake_file = os.path.join(M.path, 'wake.dat')
 
             if archive_csr_wake and os.path.exists(csr_wake_file):
                 csr_wake_data = parse_csr_wake(csr_wake_file)
                 write_csr_wake_data_h5(h5, csr_wake_data, name='csr_wake')
```

### Comparing `pytao-0.2.5/pytao/tao_ctypes/extra_commands.py` & `pytao-0.2.6/pytao/tao_ctypes/extra_commands.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/tao_ctypes/tools.py` & `pytao-0.2.6/pytao/tao_ctypes/tools.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/tao_ctypes/util.py` & `pytao-0.2.6/pytao/tao_ctypes/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,17 @@
 
     if type in ['INT', 'INUM']:
         return int(val)     
   
     if type == 'REAL':
         return float(val)
 
+    if type == 'INT_ARR':
+        return np.array(val).astype(int)
+
     if type == 'REAL_ARR':
         return np.array(val).astype(float)
 
     if type == 'COMPLEX':
         return complex(*val)
       
     if type == 'STRUCT':
```

### Comparing `pytao-0.2.5/pytao/tao_interface.py` & `pytao-0.2.6/pytao/tao_interface.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/tao_pexpect/tao_pipe.py` & `pytao-0.2.6/pytao/tao_pexpect/tao_pipe.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/tests/test_interface_commands.py` & `pytao-0.2.6/pytao/tests/test_interface_commands.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/util/data.py` & `pytao-0.2.6/pytao/util/data.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/util/evaluate_expression.py` & `pytao-0.2.6/pytao/util/evaluate_expression.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/util/lattice_element.py` & `pytao-0.2.6/pytao/util/lattice_element.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/util/parameters.py` & `pytao-0.2.6/pytao/util/parameters.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao/util/parsers.py` & `pytao-0.2.6/pytao/util/parsers.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/pytao.egg-info/PKG-INFO` & `pytao-0.2.6/pytao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytao
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://www.classe.cornell.edu/bmad/tao.html
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTao
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytao Version: 0.2.5 Home-page: https://
+Metadata-Version: 2.1 Name: pytao Version: 0.2.6 Home-page: https://
 www.classe.cornell.edu/bmad/tao.html Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE # PyTao [PyTao]((https://
 bmad-sim.github.io/pytao/index.html)) is Python interface for [Tao](https://
 www.classe.cornell.edu/bmad/tao.html), which is based on the Bmad subroutine
 library for relativistic chargedâparticle and X-ray simulations in
 accelerators and storage rings. Documentation for Bmad and Tao, as well as
 information for downloading the code if needed is given on the [Bmad website]
```

### Comparing `pytao-0.2.5/pytao.egg-info/SOURCES.txt` & `pytao-0.2.6/pytao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/setup.py` & `pytao-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.5/versioneer.py` & `pytao-0.2.6/versioneer.py`

 * *Files identical despite different names*

