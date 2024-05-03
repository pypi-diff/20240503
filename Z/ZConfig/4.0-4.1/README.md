# Comparing `tmp/ZConfig-4.0.tar.gz` & `tmp/zconfig-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZConfig-4.0.tar", last modified: Fri May  5 05:59:37 2023, max compression
+gzip compressed data, was "zconfig-4.1.tar", last modified: Fri May  3 05:25:34 2024, max compression
```

## Comparing `ZConfig-4.0.tar` & `zconfig-4.1.tar`

### file list

```diff
@@ -1,152 +1,175 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.244049 ZConfig-4.0/
--rw-r--r--   0 mac        (513) staff       (20)       80 2023-05-05 05:59:36.000000 ZConfig-4.0/.readthedocs.yml
--rw-r--r--   0 mac        (513) staff       (20)    12288 2023-05-05 05:59:36.000000 ZConfig-4.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2023-05-05 05:59:36.000000 ZConfig-4.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-05 05:59:36.000000 ZConfig-4.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-05-05 05:59:36.000000 ZConfig-4.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      530 2023-05-05 05:59:36.000000 ZConfig-4.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    17397 2023-05-05 05:59:37.244221 ZConfig-4.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     3842 2023-05-05 05:59:36.000000 ZConfig-4.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      341 2023-05-05 05:59:36.000000 ZConfig-4.0/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.209766 ZConfig-4.0/docs/
--rw-r--r--   0 mac        (513) staff       (20)      604 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)     4970 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      264 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/developing-with-zconfig.rst
--rw-r--r--   0 mac        (513) staff       (20)     2642 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/documenting-components.rst
--rw-r--r--   0 mac        (513) staff       (20)     1467 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     5339 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/logging-components.rst
--rw-r--r--   0 mac        (513) staff       (20)      811 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)      444 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-cmdline.rst
--rw-r--r--   0 mac        (513) staff       (20)      443 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-datatypes.rst
--rw-r--r--   0 mac        (513) staff       (20)     1200 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-loader.rst
--rw-r--r--   0 mac        (513) staff       (20)     2086 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-subst.rst
--rw-r--r--   0 mac        (513) staff       (20)     1922 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/py-mod-zconfig.rst
--rw-r--r--   0 mac        (513) staff       (20)      186 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/root-and-child-config.conf
--rw-r--r--   0 mac        (513) staff       (20)     3464 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/schema.dtd
--rw-r--r--   0 mac        (513) staff       (20)      131 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/simple-root-config.conf
--rw-r--r--   0 mac        (513) staff       (20)     3079 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/standard-components.rst
--rw-r--r--   0 mac        (513) staff       (20)     5829 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/standard-datatypes.rst
--rw-r--r--   0 mac        (513) staff       (20)      761 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/tools.rst
--rw-r--r--   0 mac        (513) staff       (20)     4373 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/using-logging.rst
--rw-r--r--   0 mac        (513) staff       (20)     8198 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/using-zconfig.rst
--rw-r--r--   0 mac        (513) staff       (20)     5156 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/writing-components.rst
--rw-r--r--   0 mac        (513) staff       (20)    22822 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/writing-schema.rst
--rw-r--r--   0 mac        (513) staff       (20)      159 2023-05-05 05:59:36.000000 ZConfig-4.0/docs/zconfig.rst
--rw-r--r--   0 mac        (513) staff       (20)      447 2023-05-05 05:59:37.244855 ZConfig-4.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2541 2023-05-05 05:59:36.000000 ZConfig-4.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.193939 ZConfig-4.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.215927 ZConfig-4.0/src/ZConfig/
--rw-r--r--   0 mac        (513) staff       (20)     8188 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/__init__.py
--rwxr-xr-x   0 mac        (513) staff       (20)    10563 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/_schema_utils.py
--rw-r--r--   0 mac        (513) staff       (20)     6830 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/cfgparser.py
--rw-r--r--   0 mac        (513) staff       (20)     7535 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/cmdline.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.218646 ZConfig-4.0/src/ZConfig/components/
--rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.219984 ZConfig-4.0/src/ZConfig/components/basic/
--rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      206 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/component.xml
--rw-r--r--   0 mac        (513) staff       (20)      765 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/mapping.py
--rw-r--r--   0 mac        (513) staff       (20)      945 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/mapping.xml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.220641 ZConfig-4.0/src/ZConfig/components/basic/tests/
--rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2688 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/basic/tests/test_mapping.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.225108 ZConfig-4.0/src/ZConfig/components/logger/
--rw-r--r--   0 mac        (513) staff       (20)      702 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      151 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/abstract.xml
--rw-r--r--   0 mac        (513) staff       (20)     1801 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/base-logger.xml
--rw-r--r--   0 mac        (513) staff       (20)      375 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/component.xml
--rw-r--r--   0 mac        (513) staff       (20)     1134 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/datatypes.py
--rw-r--r--   0 mac        (513) staff       (20)      478 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/eventlog.xml
--rw-r--r--   0 mac        (513) staff       (20)     1369 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/factory.py
--rw-r--r--   0 mac        (513) staff       (20)     7708 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/formatter.py
--rw-r--r--   0 mac        (513) staff       (20)     7689 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/handlers.py
--rw-r--r--   0 mac        (513) staff       (20)     9706 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/handlers.xml
--rw-r--r--   0 mac        (513) staff       (20)     3513 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/logger.py
--rw-r--r--   0 mac        (513) staff       (20)     1463 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/logger.xml
--rw-r--r--   0 mac        (513) staff       (20)     5272 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/loghandler.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.226639 ZConfig-4.0/src/ZConfig/components/logger/tests/
--rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2814 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/tests/support.py
--rw-r--r--   0 mac        (513) staff       (20)    19118 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/tests/test_formatter.py
--rw-r--r--   0 mac        (513) staff       (20)    35710 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/components/logger/tests/test_logger.py
--rw-r--r--   0 mac        (513) staff       (20)    17571 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/datatypes.py
--rw-r--r--   0 mac        (513) staff       (20)    17706 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/info.py
--rw-r--r--   0 mac        (513) staff       (20)    18005 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/loader.py
--rw-r--r--   0 mac        (513) staff       (20)    11109 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/matcher.py
--rw-r--r--   0 mac        (513) staff       (20)     2896 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/pygments.py
--rw-r--r--   0 mac        (513) staff       (20)    22431 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/schema.py
--rwxr-xr-x   0 mac        (513) staff       (20)     4626 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/schema2html.py
--rw-r--r--   0 mac        (513) staff       (20)     3168 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/schemaless.py
--rw-r--r--   0 mac        (513) staff       (20)     6887 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/schemaless.txt
--rwxr-xr-x   0 mac        (513) staff       (20)     5963 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/sphinx.py
--rw-r--r--   0 mac        (513) staff       (20)     3782 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/substitution.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.234240 ZConfig-4.0/src/ZConfig/tests/
--rw-r--r--   0 mac        (513) staff       (20)      762 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       41 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/bad-component.xml
--rw-r--r--   0 mac        (513) staff       (20)      122 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/bad-component2.xml
--rw-r--r--   0 mac        (513) staff       (20)     1581 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/foosample.zip
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.239411 ZConfig-4.0/src/ZConfig/tests/input/
--rw-r--r--   0 mac        (513) staff       (20)       98 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base-datatype1.xml
--rw-r--r--   0 mac        (513) staff       (20)       98 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base-datatype2.xml
--rw-r--r--   0 mac        (513) staff       (20)       70 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base-keytype1.xml
--rw-r--r--   0 mac        (513) staff       (20)       96 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base-keytype2.xml
--rw-r--r--   0 mac        (513) staff       (20)      161 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/base.xml
--rw-r--r--   0 mac        (513) staff       (20)       56 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/include.conf
--rw-r--r--   0 mac        (513) staff       (20)       42 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/inner.conf
--rw-r--r--   0 mac        (513) staff       (20)      157 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/library.xml
--rw-r--r--   0 mac        (513) staff       (20)      404 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/logger.xml
--rw-r--r--   0 mac        (513) staff       (20)       76 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/non-ascii.txt
--rw-r--r--   0 mac        (513) staff       (20)       62 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/outer.conf
--rw-r--r--   0 mac        (513) staff       (20)      440 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/simple.conf
--rw-r--r--   0 mac        (513) staff       (20)      951 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/simple.xml
--rw-r--r--   0 mac        (513) staff       (20)      409 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/simplesections.conf
--rw-r--r--   0 mac        (513) staff       (20)     1884 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/input/simplesections.xml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.240067 ZConfig-4.0/src/ZConfig/tests/library/
--rw-r--r--   0 mac        (513) staff       (20)       88 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/README.txt
--rw-r--r--   0 mac        (513) staff       (20)       23 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.240773 ZConfig-4.0/src/ZConfig/tests/library/thing/
--rw-r--r--   0 mac        (513) staff       (20)      840 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/thing/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      344 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/thing/component.xml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.241111 ZConfig-4.0/src/ZConfig/tests/library/thing/extras/
--rw-r--r--   0 mac        (513) staff       (20)      104 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/thing/extras/extras.xml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.242072 ZConfig-4.0/src/ZConfig/tests/library/widget/
--rw-r--r--   0 mac        (513) staff       (20)       23 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/widget/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      256 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/widget/component.xml
--rw-r--r--   0 mac        (513) staff       (20)      103 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/library/widget/extra.xml
--rw-r--r--   0 mac        (513) staff       (20)      623 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/sphinx_test_schema.xml
--rw-r--r--   0 mac        (513) staff       (20)     3553 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/support.py
--rw-r--r--   0 mac        (513) staff       (20)     3005 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_cfgimports.py
--rw-r--r--   0 mac        (513) staff       (20)     8598 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_cmdline.py
--rw-r--r--   0 mac        (513) staff       (20)    10021 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_config.py
--rw-r--r--   0 mac        (513) staff       (20)     2431 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_cookbook.py
--rw-r--r--   0 mac        (513) staff       (20)    15856 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_datatypes.py
--rw-r--r--   0 mac        (513) staff       (20)     7112 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_info.py
--rw-r--r--   0 mac        (513) staff       (20)    15547 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_loader.py
--rw-r--r--   0 mac        (513) staff       (20)     4195 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_matcher.py
--rw-r--r--   0 mac        (513) staff       (20)     8216 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_pygments.py
--rw-r--r--   0 mac        (513) staff       (20)     2704 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_readme.py
--rw-r--r--   0 mac        (513) staff       (20)    50528 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_schema.py
--rw-r--r--   0 mac        (513) staff       (20)     7660 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_schema2html.py
--rw-r--r--   0 mac        (513) staff       (20)     1277 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_schemaless.py
--rw-r--r--   0 mac        (513) staff       (20)     3771 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_subst.py
--rw-r--r--   0 mac        (513) staff       (20)     2449 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/test_validator.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.242403 ZConfig-4.0/src/ZConfig/tests/zipsource/
--rw-r--r--   0 mac        (513) staff       (20)      108 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/README.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.242734 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/
--rw-r--r--   0 mac        (513) staff       (20)       38 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.243760 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/sample/
--rw-r--r--   0 mac        (513) staff       (20)       38 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/sample/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      234 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/sample/component.xml
--rw-r--r--   0 mac        (513) staff       (20)      124 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/tests/zipsource/foo/sample/datatypes.py
--rw-r--r--   0 mac        (513) staff       (20)     1888 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/url.py
--rwxr-xr-x   0 mac        (513) staff       (20)     2167 2023-05-05 05:59:36.000000 ZConfig-4.0/src/ZConfig/validator.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 05:59:37.218326 ZConfig-4.0/src/ZConfig.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    17397 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     4282 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)      157 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/entry_points.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       92 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        8 2023-05-05 05:59:37.000000 ZConfig-4.0/src/ZConfig.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1568 2023-05-05 05:59:36.000000 ZConfig-4.0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.740962 zconfig-4.1/
+-rw-r--r--   0 jens       (501) staff       (20)      669 2024-05-02 20:48:12.000000 zconfig-4.1/.readthedocs.yaml
+-rw-r--r--   0 jens       (501) staff       (20)      160 2023-08-01 09:31:05.000000 zconfig-4.1/.readthedocs.yml
+-rw-r--r--   0 jens       (501) staff       (20)    12356 2024-05-03 05:23:34.000000 zconfig-4.1/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      804 2024-05-02 20:48:12.000000 zconfig-4.1/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:52:24.000000 zconfig-4.1/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:52:24.000000 zconfig-4.1/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      545 2024-05-02 20:48:12.000000 zconfig-4.1/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    17801 2024-05-03 05:25:34.740884 zconfig-4.1/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     3842 2023-08-01 09:31:05.000000 zconfig-4.1/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      341 2021-11-02 08:52:24.000000 zconfig-4.1/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.728694 zconfig-4.1/docs/
+-rw-r--r--   0 jens       (501) staff       (20)      604 2022-12-05 15:30:13.000000 zconfig-4.1/docs/Makefile
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.723715 zconfig-4.1/docs/_build/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.723767 zconfig-4.1/docs/_build/html/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.730515 zconfig-4.1/docs/_build/html/_sources/
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      264 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/developing-with-zconfig.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2642 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/documenting-components.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1467 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     5339 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/logging-components.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      444 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/py-mod-cmdline.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      443 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/py-mod-datatypes.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1200 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/py-mod-loader.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2086 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/py-mod-subst.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1922 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/py-mod-zconfig.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3079 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/standard-components.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     5829 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/standard-datatypes.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      761 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/tools.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     4373 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/using-logging.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     8198 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/using-zconfig.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     5156 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/writing-components.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    22822 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/writing-schema.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      159 2022-12-05 15:30:13.000000 zconfig-4.1/docs/_build/html/_sources/zconfig.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 zconfig-4.1/docs/changelog.rst
+-rw-r--r--   0 jens       (501) staff       (20)     4970 2022-12-05 15:30:13.000000 zconfig-4.1/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)      264 2022-12-05 15:30:13.000000 zconfig-4.1/docs/developing-with-zconfig.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2642 2022-12-05 15:30:13.000000 zconfig-4.1/docs/documenting-components.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1467 2022-12-05 15:30:13.000000 zconfig-4.1/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5339 2022-12-05 15:30:13.000000 zconfig-4.1/docs/logging-components.rst
+-rw-r--r--   0 jens       (501) staff       (20)      811 2022-12-05 15:30:13.000000 zconfig-4.1/docs/make.bat
+-rw-r--r--   0 jens       (501) staff       (20)      444 2022-12-05 15:30:13.000000 zconfig-4.1/docs/py-mod-cmdline.rst
+-rw-r--r--   0 jens       (501) staff       (20)      443 2022-12-05 15:30:13.000000 zconfig-4.1/docs/py-mod-datatypes.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1200 2022-12-05 15:30:13.000000 zconfig-4.1/docs/py-mod-loader.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2086 2022-12-05 15:30:13.000000 zconfig-4.1/docs/py-mod-subst.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1922 2022-12-05 15:30:13.000000 zconfig-4.1/docs/py-mod-zconfig.rst
+-rw-r--r--   0 jens       (501) staff       (20)       43 2024-05-02 20:47:48.000000 zconfig-4.1/docs/requirements.txt
+-rw-r--r--   0 jens       (501) staff       (20)      186 2022-12-05 15:30:13.000000 zconfig-4.1/docs/root-and-child-config.conf
+-rw-r--r--   0 jens       (501) staff       (20)     3464 2022-12-05 15:30:13.000000 zconfig-4.1/docs/schema.dtd
+-rw-r--r--   0 jens       (501) staff       (20)      131 2022-12-05 15:30:13.000000 zconfig-4.1/docs/simple-root-config.conf
+-rw-r--r--   0 jens       (501) staff       (20)     3079 2022-12-05 15:30:13.000000 zconfig-4.1/docs/standard-components.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5829 2022-12-05 15:30:13.000000 zconfig-4.1/docs/standard-datatypes.rst
+-rw-r--r--   0 jens       (501) staff       (20)      761 2022-12-05 15:30:13.000000 zconfig-4.1/docs/tools.rst
+-rw-r--r--   0 jens       (501) staff       (20)     4373 2022-12-05 15:30:13.000000 zconfig-4.1/docs/using-logging.rst
+-rw-r--r--   0 jens       (501) staff       (20)     8198 2022-12-05 15:30:13.000000 zconfig-4.1/docs/using-zconfig.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5156 2022-12-05 15:30:13.000000 zconfig-4.1/docs/writing-components.rst
+-rw-r--r--   0 jens       (501) staff       (20)    22822 2022-12-05 15:30:13.000000 zconfig-4.1/docs/writing-schema.rst
+-rw-r--r--   0 jens       (501) staff       (20)      159 2022-12-05 15:30:13.000000 zconfig-4.1/docs/zconfig.rst
+-rw-r--r--   0 jens       (501) staff       (20)      418 2024-05-03 05:25:34.741168 zconfig-4.1/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     2623 2024-05-03 05:23:43.000000 zconfig-4.1/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.723928 zconfig-4.1/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.732272 zconfig-4.1/src/ZConfig/
+-rw-r--r--   0 jens       (501) staff       (20)     8188 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/__init__.py
+-rwxr-xr-x   0 jens       (501) staff       (20)    10563 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/_schema_utils.py
+-rw-r--r--   0 jens       (501) staff       (20)     6830 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/cfgparser.py
+-rw-r--r--   0 jens       (501) staff       (20)     7535 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/cmdline.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.733005 zconfig-4.1/src/ZConfig/components/
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.733421 zconfig-4.1/src/ZConfig/components/basic/
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/basic/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      206 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/basic/component.xml
+-rw-r--r--   0 jens       (501) staff       (20)      765 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/basic/mapping.py
+-rw-r--r--   0 jens       (501) staff       (20)      945 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/basic/mapping.xml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.733610 zconfig-4.1/src/ZConfig/components/basic/tests/
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/basic/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     2688 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/basic/tests/test_mapping.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.734823 zconfig-4.1/src/ZConfig/components/logger/
+-rw-r--r--   0 jens       (501) staff       (20)      702 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/logger/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      151 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/logger/abstract.xml
+-rw-r--r--   0 jens       (501) staff       (20)     1801 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/logger/base-logger.xml
+-rw-r--r--   0 jens       (501) staff       (20)      375 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/logger/component.xml
+-rw-r--r--   0 jens       (501) staff       (20)     1134 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/logger/datatypes.py
+-rw-r--r--   0 jens       (501) staff       (20)      478 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/logger/eventlog.xml
+-rw-r--r--   0 jens       (501) staff       (20)     1369 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/components/logger/factory.py
+-rw-r--r--   0 jens       (501) staff       (20)     7708 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/components/logger/formatter.py
+-rw-r--r--   0 jens       (501) staff       (20)     7689 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/components/logger/handlers.py
+-rw-r--r--   0 jens       (501) staff       (20)     9706 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/components/logger/handlers.xml
+-rw-r--r--   0 jens       (501) staff       (20)     3513 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/logger/logger.py
+-rw-r--r--   0 jens       (501) staff       (20)     1463 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/logger/logger.xml
+-rw-r--r--   0 jens       (501) staff       (20)     5272 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/components/logger/loghandler.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.735260 zconfig-4.1/src/ZConfig/components/logger/tests/
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/components/logger/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     2814 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/components/logger/tests/support.py
+-rw-r--r--   0 jens       (501) staff       (20)    19118 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/components/logger/tests/test_formatter.py
+-rw-r--r--   0 jens       (501) staff       (20)    35710 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/components/logger/tests/test_logger.py
+-rw-r--r--   0 jens       (501) staff       (20)    17571 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/datatypes.py
+-rw-r--r--   0 jens       (501) staff       (20)    17706 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/info.py
+-rw-r--r--   0 jens       (501) staff       (20)    18005 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/loader.py
+-rw-r--r--   0 jens       (501) staff       (20)    11109 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/matcher.py
+-rw-r--r--   0 jens       (501) staff       (20)     2896 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/pygments.py
+-rw-r--r--   0 jens       (501) staff       (20)    22431 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/schema.py
+-rwxr-xr-x   0 jens       (501) staff       (20)     4626 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/schema2html.py
+-rw-r--r--   0 jens       (501) staff       (20)     3168 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/schemaless.py
+-rw-r--r--   0 jens       (501) staff       (20)     6887 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/schemaless.txt
+-rwxr-xr-x   0 jens       (501) staff       (20)     5963 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/sphinx.py
+-rw-r--r--   0 jens       (501) staff       (20)     3782 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/substitution.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.737465 zconfig-4.1/src/ZConfig/tests/
+-rw-r--r--   0 jens       (501) staff       (20)      762 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)       41 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/bad-component.xml
+-rw-r--r--   0 jens       (501) staff       (20)      122 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/bad-component2.xml
+-rw-r--r--   0 jens       (501) staff       (20)     1581 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/foosample.zip
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.738956 zconfig-4.1/src/ZConfig/tests/input/
+-rw-r--r--   0 jens       (501) staff       (20)       98 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/base-datatype1.xml
+-rw-r--r--   0 jens       (501) staff       (20)       98 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/base-datatype2.xml
+-rw-r--r--   0 jens       (501) staff       (20)       70 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/base-keytype1.xml
+-rw-r--r--   0 jens       (501) staff       (20)       96 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/base-keytype2.xml
+-rw-r--r--   0 jens       (501) staff       (20)      161 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/base.xml
+-rw-r--r--   0 jens       (501) staff       (20)       56 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/include.conf
+-rw-r--r--   0 jens       (501) staff       (20)       42 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/inner.conf
+-rw-r--r--   0 jens       (501) staff       (20)      157 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/library.xml
+-rw-r--r--   0 jens       (501) staff       (20)      404 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/logger.xml
+-rw-r--r--   0 jens       (501) staff       (20)       76 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/non-ascii.txt
+-rw-r--r--   0 jens       (501) staff       (20)       62 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/outer.conf
+-rw-r--r--   0 jens       (501) staff       (20)      440 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/simple.conf
+-rw-r--r--   0 jens       (501) staff       (20)      951 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/simple.xml
+-rw-r--r--   0 jens       (501) staff       (20)      409 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/simplesections.conf
+-rw-r--r--   0 jens       (501) staff       (20)     1884 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/input/simplesections.xml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.739163 zconfig-4.1/src/ZConfig/tests/library/
+-rw-r--r--   0 jens       (501) staff       (20)       88 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/library/README.txt
+-rw-r--r--   0 jens       (501) staff       (20)       23 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/library/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.739369 zconfig-4.1/src/ZConfig/tests/library/thing/
+-rw-r--r--   0 jens       (501) staff       (20)      840 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/library/thing/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      344 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/library/thing/component.xml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.739471 zconfig-4.1/src/ZConfig/tests/library/thing/extras/
+-rw-r--r--   0 jens       (501) staff       (20)      104 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/library/thing/extras/extras.xml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.739800 zconfig-4.1/src/ZConfig/tests/library/widget/
+-rw-r--r--   0 jens       (501) staff       (20)       23 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/library/widget/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      256 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/library/widget/component.xml
+-rw-r--r--   0 jens       (501) staff       (20)      103 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/library/widget/extra.xml
+-rw-r--r--   0 jens       (501) staff       (20)      623 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/sphinx_test_schema.xml
+-rw-r--r--   0 jens       (501) staff       (20)     3275 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/support.py
+-rw-r--r--   0 jens       (501) staff       (20)     3005 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_cfgimports.py
+-rw-r--r--   0 jens       (501) staff       (20)     8598 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/test_cmdline.py
+-rw-r--r--   0 jens       (501) staff       (20)    10021 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_config.py
+-rw-r--r--   0 jens       (501) staff       (20)     2431 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/test_cookbook.py
+-rw-r--r--   0 jens       (501) staff       (20)    15856 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_datatypes.py
+-rw-r--r--   0 jens       (501) staff       (20)     7112 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_info.py
+-rw-r--r--   0 jens       (501) staff       (20)    15547 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_loader.py
+-rw-r--r--   0 jens       (501) staff       (20)     4195 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_matcher.py
+-rw-r--r--   0 jens       (501) staff       (20)     8216 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_pygments.py
+-rw-r--r--   0 jens       (501) staff       (20)     2704 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_readme.py
+-rw-r--r--   0 jens       (501) staff       (20)    50528 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_schema.py
+-rw-r--r--   0 jens       (501) staff       (20)     7660 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_schema2html.py
+-rw-r--r--   0 jens       (501) staff       (20)     1277 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/test_schemaless.py
+-rw-r--r--   0 jens       (501) staff       (20)     3771 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_subst.py
+-rw-r--r--   0 jens       (501) staff       (20)     2449 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/tests/test_validator.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.739893 zconfig-4.1/src/ZConfig/tests/zipsource/
+-rw-r--r--   0 jens       (501) staff       (20)      108 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/zipsource/README.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.739995 zconfig-4.1/src/ZConfig/tests/zipsource/foo/
+-rw-r--r--   0 jens       (501) staff       (20)       38 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/zipsource/foo/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.740285 zconfig-4.1/src/ZConfig/tests/zipsource/foo/sample/
+-rw-r--r--   0 jens       (501) staff       (20)       38 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/zipsource/foo/sample/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      234 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/zipsource/foo/sample/component.xml
+-rw-r--r--   0 jens       (501) staff       (20)      124 2022-12-05 15:30:13.000000 zconfig-4.1/src/ZConfig/tests/zipsource/foo/sample/datatypes.py
+-rw-r--r--   0 jens       (501) staff       (20)     1888 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/url.py
+-rwxr-xr-x   0 jens       (501) staff       (20)     2167 2023-08-01 09:31:05.000000 zconfig-4.1/src/ZConfig/validator.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-03 05:25:34.740434 zconfig-4.1/src/ZConfig.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    17801 2024-05-03 05:25:34.000000 zconfig-4.1/src/ZConfig.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     5205 2024-05-03 05:25:34.000000 zconfig-4.1/src/ZConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-03 05:25:34.000000 zconfig-4.1/src/ZConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)      157 2024-05-03 05:25:34.000000 zconfig-4.1/src/ZConfig.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2022-12-05 15:30:57.000000 zconfig-4.1/src/ZConfig.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      109 2024-05-03 05:25:34.000000 zconfig-4.1/src/ZConfig.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        8 2024-05-03 05:25:34.000000 zconfig-4.1/src/ZConfig.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2012 2024-05-03 05:16:45.000000 zconfig-4.1/tox.ini
```

### Comparing `ZConfig-4.0/CHANGES.rst` & `zconfig-4.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ============================
  Change History for ZConfig
 ============================
 
+4.1 (2024-05-03)
+================
+
+- Add support for Python 3.12.
+
+
 4.0 (2023-05-05)
 ================
 
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 3.6.1 (2022-12-06)
```

### Comparing `ZConfig-4.0/CONTRIBUTING.md` & `zconfig-4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/LICENSE.txt` & `zconfig-4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/MANIFEST.in` & `zconfig-4.1/MANIFEST.in`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
 
 recursive-include src *.py
+include *.yaml
 include *.yml
 recursive-include docs *.bat
 recursive-include docs *.conf
 recursive-include docs *.dtd
 recursive-include src *.conf
 recursive-include src *.txt
 recursive-include src *.xml
```

### Comparing `ZConfig-4.0/PKG-INFO` & `zconfig-4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZConfig
-Version: 4.0
+Version: 4.1
 Summary: Structured Configuration Library
 Home-page: https://github.com/zopefoundation/ZConfig/
 Author: Fred L. Drake, Jr.
 Author-email: fred@fdrake.net
 Maintainer: Zope Foundation and Contributors
 License: ZPL 2.1
 Keywords: configuration structured simple flexible typed hierarchy logging
@@ -16,22 +16,29 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
+License-File: LICENSE.txt
 Provides-Extra: test
+Requires-Dist: docutils; extra == "test"
+Requires-Dist: manuel; extra == "test"
+Requires-Dist: zope.exceptions; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 Provides-Extra: docs
-License-File: LICENSE.txt
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 
 ZConfig: Schema-driven configuration
 ====================================
 
 .. image:: https://img.shields.io/pypi/v/ZConfig.svg
         :target: https://pypi.python.org/pypi/ZConfig/
         :alt: Latest release
@@ -141,14 +148,20 @@
 `Python Packaging User Guide <https://packaging.python.org/>`__.
 
 
 ============================
  Change History for ZConfig
 ============================
 
+4.1 (2024-05-03)
+================
+
+- Add support for Python 3.12.
+
+
 4.0 (2023-05-05)
 ================
 
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 3.6.1 (2022-12-06)
```

### Comparing `ZConfig-4.0/README.rst` & `zconfig-4.1/README.rst`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/Makefile` & `zconfig-4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/conf.py` & `zconfig-4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/documenting-components.rst` & `zconfig-4.1/docs/_build/html/_sources/documenting-components.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/index.rst` & `zconfig-4.1/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/logging-components.rst` & `zconfig-4.1/docs/_build/html/_sources/logging-components.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/make.bat` & `zconfig-4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/py-mod-loader.rst` & `zconfig-4.1/docs/_build/html/_sources/py-mod-loader.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/py-mod-subst.rst` & `zconfig-4.1/docs/_build/html/_sources/py-mod-subst.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/py-mod-zconfig.rst` & `zconfig-4.1/docs/_build/html/_sources/py-mod-zconfig.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/schema.dtd` & `zconfig-4.1/docs/schema.dtd`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/standard-components.rst` & `zconfig-4.1/docs/_build/html/_sources/standard-components.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/standard-datatypes.rst` & `zconfig-4.1/docs/_build/html/_sources/standard-datatypes.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/tools.rst` & `zconfig-4.1/docs/_build/html/_sources/tools.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/using-logging.rst` & `zconfig-4.1/docs/_build/html/_sources/using-logging.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/using-zconfig.rst` & `zconfig-4.1/docs/_build/html/_sources/using-zconfig.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/writing-components.rst` & `zconfig-4.1/docs/_build/html/_sources/writing-components.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/docs/writing-schema.rst` & `zconfig-4.1/docs/_build/html/_sources/writing-schema.rst.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/setup.py` & `zconfig-4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'manuel',
     'zope.exceptions',
     'zope.testrunner',
 ]
 
 setup(
     name="ZConfig",
-    version='4.0',
+    version='4.1',
     author="Fred L. Drake, Jr.",
     author_email="fred@fdrake.net",
     maintainer="Zope Foundation and Contributors",
     description="Structured Configuration Library",
     keywords=('configuration structured simple flexible typed hierarchy'
               ' logging'),
     long_description=README + "\n\n" + CHANGES,
@@ -63,20 +63,22 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: OS Independent',
         'Topic :: Software Development',
     ],
     python_requires='>=3.7',
     extras_require={
         'test': tests_require,
         'docs': [
+            'sphinx-rtd-theme',
             'sphinxcontrib-programoutput',
         ],
     },
 )
```

### Comparing `ZConfig-4.0/src/ZConfig/__init__.py` & `zconfig-4.1/src/ZConfig/__init__.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/_schema_utils.py` & `zconfig-4.1/src/ZConfig/_schema_utils.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/cfgparser.py` & `zconfig-4.1/src/ZConfig/cfgparser.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/cmdline.py` & `zconfig-4.1/src/ZConfig/cmdline.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/basic/mapping.py` & `zconfig-4.1/src/ZConfig/components/basic/mapping.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/basic/mapping.xml` & `zconfig-4.1/src/ZConfig/components/basic/mapping.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/basic/tests/test_mapping.py` & `zconfig-4.1/src/ZConfig/components/basic/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/__init__.py` & `zconfig-4.1/src/ZConfig/components/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/base-logger.xml` & `zconfig-4.1/src/ZConfig/components/logger/base-logger.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/datatypes.py` & `zconfig-4.1/src/ZConfig/components/logger/datatypes.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/factory.py` & `zconfig-4.1/src/ZConfig/components/logger/factory.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/formatter.py` & `zconfig-4.1/src/ZConfig/components/logger/formatter.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/handlers.py` & `zconfig-4.1/src/ZConfig/components/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/handlers.xml` & `zconfig-4.1/src/ZConfig/components/logger/handlers.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/logger.py` & `zconfig-4.1/src/ZConfig/components/logger/logger.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/logger.xml` & `zconfig-4.1/src/ZConfig/components/logger/logger.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/loghandler.py` & `zconfig-4.1/src/ZConfig/components/logger/loghandler.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/tests/support.py` & `zconfig-4.1/src/ZConfig/components/logger/tests/support.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/tests/test_formatter.py` & `zconfig-4.1/src/ZConfig/components/logger/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/components/logger/tests/test_logger.py` & `zconfig-4.1/src/ZConfig/components/logger/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/datatypes.py` & `zconfig-4.1/src/ZConfig/datatypes.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/info.py` & `zconfig-4.1/src/ZConfig/info.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/loader.py` & `zconfig-4.1/src/ZConfig/loader.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/matcher.py` & `zconfig-4.1/src/ZConfig/matcher.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/pygments.py` & `zconfig-4.1/src/ZConfig/pygments.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/schema.py` & `zconfig-4.1/src/ZConfig/schema.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/schema2html.py` & `zconfig-4.1/src/ZConfig/schema2html.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/schemaless.py` & `zconfig-4.1/src/ZConfig/schemaless.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/schemaless.txt` & `zconfig-4.1/src/ZConfig/schemaless.txt`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/sphinx.py` & `zconfig-4.1/src/ZConfig/sphinx.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/substitution.py` & `zconfig-4.1/src/ZConfig/substitution.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/__init__.py` & `zconfig-4.1/src/ZConfig/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/foosample.zip` & `zconfig-4.1/src/ZConfig/tests/foosample.zip`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/input/simple.xml` & `zconfig-4.1/src/ZConfig/tests/input/simple.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/input/simplesections.xml` & `zconfig-4.1/src/ZConfig/tests/input/simplesections.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/library/thing/__init__.py` & `zconfig-4.1/src/ZConfig/tests/library/thing/__init__.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/sphinx_test_schema.xml` & `zconfig-4.1/src/ZConfig/tests/sphinx_test_schema.xml`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/support.py` & `zconfig-4.1/src/ZConfig/tests/support.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 ##############################################################################
 
 """Support code shared among the tests."""
 
 import contextlib
 import os
 import sys
-import unittest
 from io import StringIO
 from urllib.request import pathname2url
 
 import ZConfig
 from ZConfig.loader import ConfigLoader
 from ZConfig.url import urljoin
 
@@ -75,20 +74,14 @@
 
     return make_wrapper
 
 
 class TestHelper:
     """Utility methods which can be used with the schema support."""
 
-    # Not derived from unittest.TestCase; some test runners seem to
-    # think that means this class contains tests.
-
-    assertRaisesRegex = getattr(unittest.TestCase, 'assertRaisesRegex',
-                                unittest.TestCase.assertRaisesRegexp)
-
     def load_both(self, schema_url, conf_url):
         schema = self.load_schema(schema_url)
         conf = self.load_config(schema, conf_url)
         return schema, conf
 
     def load_schema(self, relurl):
         self.url = urljoin(CONFIG_BASE, relurl)
```

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_cfgimports.py` & `zconfig-4.1/src/ZConfig/tests/test_cfgimports.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_cmdline.py` & `zconfig-4.1/src/ZConfig/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_config.py` & `zconfig-4.1/src/ZConfig/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_cookbook.py` & `zconfig-4.1/src/ZConfig/tests/test_cookbook.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_datatypes.py` & `zconfig-4.1/src/ZConfig/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_info.py` & `zconfig-4.1/src/ZConfig/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_loader.py` & `zconfig-4.1/src/ZConfig/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_matcher.py` & `zconfig-4.1/src/ZConfig/tests/test_matcher.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_pygments.py` & `zconfig-4.1/src/ZConfig/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_readme.py` & `zconfig-4.1/src/ZConfig/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_schema.py` & `zconfig-4.1/src/ZConfig/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_schema2html.py` & `zconfig-4.1/src/ZConfig/tests/test_schema2html.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_schemaless.py` & `zconfig-4.1/src/ZConfig/tests/test_schemaless.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_subst.py` & `zconfig-4.1/src/ZConfig/tests/test_subst.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/tests/test_validator.py` & `zconfig-4.1/src/ZConfig/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/url.py` & `zconfig-4.1/src/ZConfig/url.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig/validator.py` & `zconfig-4.1/src/ZConfig/validator.py`

 * *Files identical despite different names*

### Comparing `ZConfig-4.0/src/ZConfig.egg-info/PKG-INFO` & `zconfig-4.1/src/ZConfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZConfig
-Version: 4.0
+Version: 4.1
 Summary: Structured Configuration Library
 Home-page: https://github.com/zopefoundation/ZConfig/
 Author: Fred L. Drake, Jr.
 Author-email: fred@fdrake.net
 Maintainer: Zope Foundation and Contributors
 License: ZPL 2.1
 Keywords: configuration structured simple flexible typed hierarchy logging
@@ -16,22 +16,29 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
+License-File: LICENSE.txt
 Provides-Extra: test
+Requires-Dist: docutils; extra == "test"
+Requires-Dist: manuel; extra == "test"
+Requires-Dist: zope.exceptions; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 Provides-Extra: docs
-License-File: LICENSE.txt
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 
 ZConfig: Schema-driven configuration
 ====================================
 
 .. image:: https://img.shields.io/pypi/v/ZConfig.svg
         :target: https://pypi.python.org/pypi/ZConfig/
         :alt: Latest release
@@ -141,14 +148,20 @@
 `Python Packaging User Guide <https://packaging.python.org/>`__.
 
 
 ============================
  Change History for ZConfig
 ============================
 
+4.1 (2024-05-03)
+================
+
+- Add support for Python 3.12.
+
+
 4.0 (2023-05-05)
 ================
 
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 3.6.1 (2022-12-06)
```

### Comparing `ZConfig-4.0/tox.ini` & `zconfig-4.1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
+    release-check
     lint
     py37
     py38
     py39
     py310
     py311
+    py312
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
+package = wheel
+wheel_build_env = .pkg
 deps =
+setenv =
+    py312: VIRTUALENV_PIP=23.1.2
+    py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
+[testenv:release-check]
+description = ensure that the distribution is ready to release
+basepython = python3
+skip_install = true
+deps =
+    twine
+    build
+    check-manifest
+    check-python-versions >= 0.20.0
+    wheel
+commands_pre =
+commands =
+    check-manifest
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
+    python -m build --sdist --no-isolation
+    twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+deps =
+    isort
+    flake8
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 src setup.py
-    check-manifest
-    check-python-versions
-deps =
-    check-manifest
-    check-python-versions >= 0.19.1
-    wheel
-    flake8
-    isort
 
 [testenv:isort-apply]
 basepython = python3
 skip_install = true
 commands_pre =
 deps =
     isort
```

