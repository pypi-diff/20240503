# Comparing `tmp/ophyd_async-0.3a2.tar.gz` & `tmp/ophyd_async-0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd_async-0.3a2.tar", last modified: Tue Apr 23 14:45:33 2024, max compression
+gzip compressed data, was "ophyd_async-0.3a3.tar", last modified: Fri May  3 13:43:33 2024, max compression
```

## Comparing `ophyd_async-0.3a2.tar` & `ophyd_async-0.3a3.tar`

### file list

```diff
@@ -1,225 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.887047 ophyd_async-0.3a2/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.859047 ophyd_async-0.3a2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.859047 ophyd_async-0.3a2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.855047 ophyd_async-0.3a2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.859047 ophyd_async-0.3a2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.859047 ophyd_async-0.3a2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-23 14:45:33.887047 ophyd_async-0.3a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/_templates/README
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/examples/epics_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0003-ophyd-async-migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0004-repository-structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0005-respect-black-line-length.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0006-procedural-device-definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/event-loop-choice.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to/compound-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to/make-a-simple-device.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to/write-tests-for-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.867047 ophyd_async-0.3a2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/images/bluesky_ophyd_epics_devices_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/images/bluesky_ophyd_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/images/ophyd_favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.867047 ophyd_async-0.3a2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.867047 ophyd_async-0.3a2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/tutorials/using-existing-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:45:33.887047 ophyd_async-0.3a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.855047 ophyd_async-0.3a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.867047 ophyd_async-0.3a2/src/ophyd_async/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/sim_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/_aioca.py
--rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/_p4p.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/aravis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/ad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/_hdffile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/demo/mover.db
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/demo/sensor.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/motion/motor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/epics/pvi/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/pvi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/pvi/pvi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/epics/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/signal/_epics_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/signal/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/panda/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_common_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/panda/writers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/writers/_hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/writers/_panda_hdf_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/planstubs/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/planstubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/planstubs/prepare_trigger_and_dets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/demo/sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/sim_pattern_detector_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/sim_pattern_detector_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/sim_pattern_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/src/ophyd_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_device_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/epics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/_backend/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_aravis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/demo/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/demo/test_demo_ad_sim_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/motion/test_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/test_pvi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/test_records.db
--rw-r--r--   0 runner    (1001) docker     (127)    17239 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/test_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/panda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/panda/db/
--rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/db/panda.db
--rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_panda_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_panda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/protocols/test_protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/sim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/demo/test_sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/test_pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/test_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/test_sim_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/test_streaming_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/test_flyer_with_panda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.663325 ophyd_async-0.3a3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/_templates/README
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/examples/epics_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/examples/foo_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0003-ophyd-async-migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0004-repository-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0005-respect-black-line-length.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0006-procedural-device-definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/design-goals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/event-loop-choice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/flyscanning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/choose-interfaces-for-devices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/compound-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/make-a-simple-device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/make-a-standard-detector.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/write-tests-for-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/bluesky_ophyd_epics_devices_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/bluesky_ophyd_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   253748 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/hardware-triggered-scan.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/ophyd_favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    89951 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/outer-scan.png
+-rw-r--r--   0 runner    (1001) docker     (127)   128990 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/simple-hardware-scan.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/tutorials/using-existing-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.667325 ophyd_async-0.3a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/src/ophyd_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.683325 ophyd_async-0.3a3/src/ophyd_async/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/sim_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.683325 ophyd_async-0.3a3/src/ophyd_async/epics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.683325 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/_aioca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/_p4p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.687325 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/aravis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.687325 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.687325 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/ad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/vimba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.687325 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/_hdffile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/demo/mover.db
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/demo/sensor.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/motion/motor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/epics/pvi/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/pvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/pvi/pvi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/epics/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/signal/_epics_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/signal/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/panda/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_common_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/panda/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/writers/_hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/writers/_panda_hdf_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/planstubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/planstubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/planstubs/prepare_trigger_and_dets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/src/ophyd_async/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/src/ophyd_async/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/demo/sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_detector_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_detector_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/src/ophyd_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_device_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/tests/epics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/tests/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/_backend/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_aravis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_vimba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/demo/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/demo/test_demo_ad_sim_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/motion/test_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/test_pvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/test_records.db
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/panda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/panda/db/
+-rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/db/panda.db
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_panda_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_panda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/protocols/test_protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/tests/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/demo/test_sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/test_pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/test_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/test_sim_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/test_streaming_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/test_flyer_with_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/test_log.py
```

### Comparing `ophyd_async-0.3a2/.devcontainer/devcontainer.json` & `ophyd_async-0.3a3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.github/CONTRIBUTING.md` & `ophyd_async-0.3a3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.github/actions/install_requirements/action.yml` & `ophyd_async-0.3a3/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.github/dependabot.yml` & `ophyd_async-0.3a3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.github/pages/make_switcher.py` & `ophyd_async-0.3a3/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.github/workflows/_check.yml` & `ophyd_async-0.3a3/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.github/workflows/_dist.yml` & `ophyd_async-0.3a3/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.github/workflows/_docs.yml` & `ophyd_async-0.3a3/.github/workflows/_docs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -43,12 +43,12 @@
       - name: Write switcher.json
         run: python .github/pages/make_switcher.py --add $DOCS_VERSION ${{ github.repository }} .github/pages/switcher.json
 
       - name: Publish Docs to gh-pages
         if: github.ref_type == 'tag' || github.ref_name == 'main'
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: peaceiris/actions-gh-pages@373f7f263a76c20808c831209c920827a82a2847 # v3.9.3
+        uses: peaceiris/actions-gh-pages@4f9cc6602d3f66b9c108549d475ec49e8ef4d45e # v4.0.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
```

### Comparing `ophyd_async-0.3a2/.github/workflows/_release.yml` & `ophyd_async-0.3a3/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.github/workflows/_test.yml` & `ophyd_async-0.3a3/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.github/workflows/ci.yml` & `ophyd_async-0.3a3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.gitignore` & `ophyd_async-0.3a3/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.mailmap` & `ophyd_async-0.3a3/.mailmap`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/.pre-commit-config.yaml` & `ophyd_async-0.3a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/Dockerfile` & `ophyd_async-0.3a3/Dockerfile`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/LICENSE` & `ophyd_async-0.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/PKG-INFO` & `ophyd_async-0.3a3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a2
+Version: 0.3a3
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
@@ -68,40 +68,57 @@
 Requires-Dist: numpydoc; extra == "dev"
 Requires-Dist: ophyd; extra == "dev"
 Requires-Dist: pickleshare; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: pyepics>=3.4.2; extra == "dev"
-Requires-Dist: pyside6==6.6.2; extra == "dev"
+Requires-Dist: pyside6==6.7.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-faulthandler; extra == "dev"
 Requires-Dist: pytest-rerunfailures; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
+Requires-Dist: sphinxcontrib-mermaid; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
+Requires-Dist: colorlog; extra == "dev"
 
 [![CI](https://github.com/bluesky/ophyd-async/actions/workflows/ci.yml/badge.svg)](https://github.com/bluesky/ophyd-async/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/bluesky/ophyd-async/branch/main/graph/badge.svg)](https://codecov.io/gh/bluesky/ophyd-async)
 [![PyPI](https://img.shields.io/pypi/v/ophyd-async.svg)](https://pypi.org/project/ophyd-async)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-# ophyd_async
+# ophyd-async
 
 Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 
 |    Source     |     <https://github.com/bluesky/ophyd-async>      |
 | :-----------: | :-----------------------------------------------: |
 |     PyPI      |             `pip install ophyd-async`             |
 | Documentation |      <https://bluesky.github.io/ophyd-async>      |
 |   Releases    | <https://github.com/bluesky/ophyd-async/releases> |
 
+Ophyd-async is a Python library for asynchronously interfacing with hardware, intended to 
+be used as an abstraction layer that enables experiment orchestration and data acquisition code to operate above the specifics of particular devices and control
+systems.
+
+Both ophyd and ophyd-async are typically used with the [Bluesky Run Engine][] for experiment orchestration and data acquisition.
+
+While [EPICS][] is the most common control system layer that ophyd-async can interface with, support for other control systems like [Tango][] will be supported in the future. The focus of ophyd-async is:
+
+* Asynchronous signal access, opening the possibility for hardware-triggered scanning (also known as fly-scanning)
+* Simpler instantiation of devices (groupings of signals) with less reliance upon complex class hierarchies
+
+[Bluesky Run Engine]: http://blueskyproject.io/bluesky
+[EPICS]: http://www.aps.anl.gov/epics/
+[Tango]: https://www.tango-controls.org/
+
 <!-- README only content. Anything below this line won't be included in index.md -->
 
 See https://bluesky.github.io/ophyd-async for more detailed documentation.
```

### Comparing `ophyd_async-0.3a2/docs/_templates/custom-class-template.rst` & `ophyd_async-0.3a3/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/_templates/custom-module-template.rst` & `ophyd_async-0.3a3/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/conf.py` & `ophyd_async-0.3a3/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     root = Path(__file__).absolute().parent.parent
     git_branch = check_output("git branch --show-current".split(), cwd=root)
     version = git_branch.decode().strip()
 else:
     version = release
 
 extensions = [
+    # for diagrams
+    "sphinxcontrib.mermaid",
     # Use this for generating API docs
     "sphinx.ext.autodoc",
     "sphinx.ext.doctest",
     # This can parse google style docstrings
     "sphinx.ext.napoleon",
     # For linking to external sphinx documentation
     "sphinx.ext.intersphinx",
@@ -53,14 +55,17 @@
     "IPython.sphinxext.ipython_directive",
     "IPython.sphinxext.ipython_console_highlighting",
     "matplotlib.sphinxext.plot_directive",
     "myst_parser",
     "numpydoc",
 ]
 
+# So we can use the ::: syntax
+myst_enable_extensions = ["colon_fence"]
+
 napoleon_google_docstring = False
 napoleon_numpy_docstring = True
 
 # If true, Sphinx will warn about all references where the target cannot
 # be found.
 # nitpicky = True
 
@@ -180,35 +185,26 @@
     "github_url": f"https://github.com/{github_user}/{github_repo}",
     "icon_links": [
         {
             "name": "PyPI",
             "url": f"https://pypi.org/project/{project}",
             "icon": "fas fa-cube",
         },
-        {
-            "name": "Gitter",
-            "url": "https://gitter.im/NSLS-II/DAMA",
-            "icon": "fas fa-person-circle-question",
-        },
     ],
     "switcher": {
         "json_url": switcher_json,
         "version_match": version,
     },
     "check_switcher": False,
     "navbar_end": ["theme-switcher", "icon-links", "version-switcher"],
     "external_links": [
         {
             "name": "Bluesky Project",
             "url": "https://blueskyproject.io",
         },
-        {
-            "name": "Release Notes",
-            "url": f"https://github.com/{github_user}/{github_repo}/releases",
-        },
     ],
     "navigation_with_keys": False,
 }
 
 # A dictionary of values to pass into the template engine’s context for all pages
 html_context = {
     "github_user": github_user,
```

### Comparing `ophyd_async-0.3a2/docs/examples/epics_demo.py` & `ophyd_async-0.3a3/docs/examples/epics_demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `ophyd_async-0.3a3/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/explanations/decisions/0003-ophyd-async-migration.rst` & `ophyd_async-0.3a3/docs/explanations/decisions/0003-ophyd-async-migration.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/explanations/decisions/0004-repository-structure.rst` & `ophyd_async-0.3a3/docs/explanations/decisions/0004-repository-structure.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/explanations/decisions/0005-respect-black-line-length.rst` & `ophyd_async-0.3a3/docs/explanations/decisions/0005-respect-black-line-length.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/explanations/decisions/0006-procedural-device-definitions.rst` & `ophyd_async-0.3a3/docs/explanations/decisions/0006-procedural-device-definitions.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/explanations/event-loop-choice.rst` & `ophyd_async-0.3a3/docs/explanations/event-loop-choice.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/how-to/compound-devices.rst` & `ophyd_async-0.3a3/docs/how-to/compound-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/how-to/make-a-simple-device.rst` & `ophyd_async-0.3a3/docs/how-to/make-a-simple-device.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/how-to/write-tests-for-devices.rst` & `ophyd_async-0.3a3/docs/how-to/write-tests-for-devices.rst`

 * *Files 22% similar despite different names*

```diff
@@ -31,15 +31,26 @@
 
 
 Sim Utility Functions
 ---------------------
 
 Sim signals behave as simply as possible, holding a sensible default value when initialized and retaining any value (in memory) to which they are set. This model breaks down in the case of read-only signals, which cannot be set because there is an expectation of some external device setting them in the real world. There is a utility function, ``set_sim_value``, to mock-set values for sim signals, including read-only ones.
 
+In addition this example also utilizes helper functions like ``assert_reading`` and ``assert_value`` to ensure the validity of device readings and values. For more information see: :doc:`API.core<../generated/ophyd_async.core>`
+
 .. literalinclude:: ../../tests/epics/demo/test_demo.py
    :pyobject: test_sensor_reading_shows_value
 
 
 There is another utility function, ``set_sim_callback``, for hooking in logic when a sim value changes (e.g. because someone puts to it).
 
 .. literalinclude:: ../../tests/epics/demo/test_demo.py
    :pyobject: test_mover_stopped
+
+
+Testing a Device in a Plan with the RunEngine
+---------------------------------------------
+.. literalinclude:: ../../tests/epics/demo/test_demo.py
+   :pyobject: test_sensor_in_plan
+
+
+This test verifies that the sim_sensor behaves as expected within a plan. The plan we use here is a ``count``, which takes a specified number of readings from the ``sim_sensor``. Since we set the ``repeat`` to two in this test, the sensor should emit two "event" documents along with "start", "stop" and "descriptor" documents. Finally, we use the helper function ``assert_emitted`` to confirm that the emitted documents match our expectations.
```

### Comparing `ophyd_async-0.3a2/docs/images/bluesky_ophyd_epics_devices_logo.svg` & `ophyd_async-0.3a3/docs/images/bluesky_ophyd_epics_devices_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/images/bluesky_ophyd_logo.svg` & `ophyd_async-0.3a3/docs/images/bluesky_ophyd_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/images/ophyd_favicon.svg` & `ophyd_async-0.3a3/docs/images/ophyd_favicon.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/index.md` & `ophyd_async-0.3a3/docs/index.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/reference/api.rst` & `ophyd_async-0.3a3/docs/reference/api.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/tutorials/installation.md` & `ophyd_async-0.3a3/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/docs/tutorials/using-existing-devices.rst` & `ophyd_async-0.3a3/docs/tutorials/using-existing-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/pyproject.toml` & `ophyd_async-0.3a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -45,28 +45,30 @@
     "numpydoc",
     "ophyd",
     "pickleshare",
     "pipdeptree",
     "pre-commit",
     "pydata-sphinx-theme>=0.12",
     "pyepics>=3.4.2",
-    "pyside6==6.6.2",
+    "pyside6==6.7.0",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-faulthandler",
     "pytest-rerunfailures",
     "pytest-timeout",
     "ruff",
     "sphinx-autobuild",
+    "sphinxcontrib-mermaid",
     "sphinx-copybutton",
     "sphinx-design",
     "tox-direct",
     "types-mock",
     "types-pyyaml",
+    "colorlog"
 ]
 
 [project.scripts]
 ophyd-async = "ophyd_async.__main__:main"
 
 [project.urls]
 GitHub = "https://github.com/bluesky/ophyd-async"
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/__init__.py` & `ophyd_async-0.3a3/src/ophyd_async/core/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,26 +26,30 @@
 from .flyer import HardwareTriggeredFlyable, TriggerLogic
 from .signal import (
     Signal,
     SignalR,
     SignalRW,
     SignalW,
     SignalX,
+    assert_configuration,
+    assert_emitted,
+    assert_reading,
+    assert_value,
     observe_value,
     set_and_wait_for_value,
     set_sim_callback,
     set_sim_put_proceeds,
     set_sim_value,
     soft_signal_r_and_backend,
     soft_signal_rw,
     wait_for_value,
 )
 from .signal_backend import SignalBackend
 from .sim_signal_backend import SimSignalBackend
-from .standard_readable import StandardReadable
+from .standard_readable import ConfigSignal, HintedSignal, StandardReadable
 from .utils import (
     DEFAULT_TIMEOUT,
     Callback,
     NotConnected,
     ReadingValueCallback,
     T,
     get_dtype,
@@ -80,14 +84,16 @@
     "AsyncStatus",
     "DirectoryInfo",
     "DirectoryProvider",
     "NameProvider",
     "ShapeProvider",
     "StaticDirectoryProvider",
     "StandardReadable",
+    "ConfigSignal",
+    "HintedSignal",
     "TriggerInfo",
     "TriggerLogic",
     "HardwareTriggeredFlyable",
     "DEFAULT_TIMEOUT",
     "Callback",
     "NotConnected",
     "ReadingValueCallback",
@@ -99,8 +105,12 @@
     "get_signal_values",
     "load_from_yaml",
     "save_to_yaml",
     "set_signal_values",
     "walk_rw_signals",
     "load_device",
     "save_device",
+    "assert_reading",
+    "assert_value",
+    "assert_configuration",
+    "assert_emitted",
 ]
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/_providers.py` & `ophyd_async-0.3a3/src/ophyd_async/core/_providers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/async_status.py` & `ophyd_async-0.3a3/src/ophyd_async/core/async_status.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/detector.py` & `ophyd_async-0.3a3/src/ophyd_async/core/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,28 @@
     Optional,
     Sequence,
     TypeVar,
 )
 
 from bluesky.protocols import (
     Collectable,
-    Descriptor,
+    DataKey,
     Flyable,
     Preparable,
     Reading,
     Stageable,
     StreamAsset,
     Triggerable,
     WritesStreamAssets,
 )
 
 from ophyd_async.protocols import AsyncConfigurable, AsyncReadable
 
 from .async_status import AsyncStatus
 from .device import Device
-from .signal import SignalR
 from .utils import DEFAULT_TIMEOUT, merge_gathered_dicts
 
 T = TypeVar("T")
 
 
 class DetectorTrigger(str, Enum):
     """Type of mechanism for triggering a detector to take frames"""
@@ -106,15 +105,15 @@
 
 
 class DetectorWriter(ABC):
     """Logic for making a detector write data to somewhere persistent
     (e.g. an HDF5 file)"""
 
     @abstractmethod
-    async def open(self, multiplier: int = 1) -> Dict[str, Descriptor]:
+    async def open(self, multiplier: int = 1) -> Dict[str, DataKey]:
         """Open writer and wait for it to be ready for data.
 
         Args:
             multiplier: Each StreamDatum index corresponds to this many
                 written exposures
 
         Returns:
@@ -157,15 +156,15 @@
     Aggregates controller and writer logic together.
     """
 
     def __init__(
         self,
         controller: DetectorControl,
         writer: DetectorWriter,
-        config_sigs: Sequence[SignalR] = (),
+        config_sigs: Sequence[AsyncReadable] = (),
         name: str = "",
         writer_timeout: float = DEFAULT_TIMEOUT,
     ) -> None:
         """
         Constructor
 
         Args:
@@ -177,15 +176,15 @@
             writer_timeout: Timeout for frame writing to start, if the
             timeout is reached, ophyd-async assumes the detector
             has a problem and raises an error.
             Defaults to DEFAULT_TIMEOUT.
         """
         self._controller = controller
         self._writer = writer
-        self._describe: Dict[str, Descriptor] = {}
+        self._describe: Dict[str, DataKey] = {}
         self._config_sigs = list(config_sigs)
         self._frame_writing_timeout = writer_timeout
         # For prepare
         self._arm_status: Optional[AsyncStatus] = None
         self._trigger_info: Optional[TriggerInfo] = None
         # For kickoff
         self._watchers: List[Callable] = []
@@ -210,15 +209,15 @@
         await self._check_config_sigs()
         await asyncio.gather(self.writer.close(), self.controller.disarm())
         self._describe = await self.writer.open()
 
     async def _check_config_sigs(self):
         """Checks configuration signals are named and connected."""
         for signal in self._config_sigs:
-            if signal._name == "":
+            if signal.name == "":
                 raise Exception(
                     "config signal must be named before it is passed to the detector"
                 )
             try:
                 await signal.get_value()
             except NotImplementedError:
                 raise Exception(
@@ -230,22 +229,22 @@
     async def unstage(self) -> None:
         # Stop data writing.
         await self.writer.close()
 
     async def read_configuration(self) -> Dict[str, Reading]:
         return await merge_gathered_dicts(sig.read() for sig in self._config_sigs)
 
-    async def describe_configuration(self) -> Dict[str, Descriptor]:
+    async def describe_configuration(self) -> Dict[str, DataKey]:
         return await merge_gathered_dicts(sig.describe() for sig in self._config_sigs)
 
     async def read(self) -> Dict[str, Reading]:
         # All data is in StreamResources, not Events, so nothing to output here
         return {}
 
-    async def describe(self) -> Dict[str, Descriptor]:
+    async def describe(self) -> Dict[str, DataKey]:
         return self._describe
 
     @AsyncStatus.wrap
     async def trigger(self) -> None:
         # Arm the detector and wait for it to finish.
         indices_written = await self.writer.get_indices_written()
         written_status = await self.controller.arm(
@@ -326,15 +325,15 @@
                 break
 
     @AsyncStatus.wrap
     async def complete(self) -> AsyncStatus:
         assert self._fly_status, "Kickoff not run"
         return await self._fly_status
 
-    async def describe_collect(self) -> Dict[str, Descriptor]:
+    async def describe_collect(self) -> Dict[str, DataKey]:
         return self._describe
 
     async def collect_asset_docs(
         self, index: Optional[int] = None
     ) -> AsyncIterator[StreamAsset]:
         # Collect stream datum documents for all indices written.
         # The index is optional, and provided for fly scans, however this needs to be
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/device.py` & `ophyd_async-0.3a3/src/ophyd_async/core/device.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/device_save_loader.py` & `ophyd_async-0.3a3/src/ophyd_async/core/device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/flyer.py` & `ophyd_async-0.3a3/src/ophyd_async/core/flyer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Generic, Sequence, TypeVar
 
-from bluesky.protocols import Descriptor, Flyable, Preparable, Reading, Stageable
+from bluesky.protocols import DataKey, Flyable, Preparable, Reading, Stageable
 
 from .async_status import AsyncStatus
 from .device import Device
 from .signal import SignalR
 from .utils import merge_gathered_dicts
 
 T = TypeVar("T")
@@ -70,15 +70,15 @@
     async def kickoff(self) -> None:
         await self._trigger_logic.kickoff()
 
     @AsyncStatus.wrap
     async def complete(self) -> None:
         await self._trigger_logic.complete()
 
-    async def describe_configuration(self) -> Dict[str, Descriptor]:
+    async def describe_configuration(self) -> Dict[str, DataKey]:
         return await merge_gathered_dicts(
             [sig.describe() for sig in self._configuration_signals]
         )
 
     async def read_configuration(self) -> Dict[str, Reading]:
         return await merge_gathered_dicts(
             [sig.read() for sig in self._configuration_signals]
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/signal.py` & `ophyd_async-0.3a3/src/ophyd_async/core/signal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 from __future__ import annotations
 
 import asyncio
 import functools
-from typing import AsyncGenerator, Callable, Dict, Generic, Optional, Tuple, Type, Union
+from typing import (
+    Any,
+    AsyncGenerator,
+    Callable,
+    Dict,
+    Generic,
+    Mapping,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
 
 from bluesky.protocols import (
-    Descriptor,
+    DataKey,
     Locatable,
     Location,
     Movable,
     Reading,
-    Stageable,
     Subscribable,
 )
 
-from ophyd_async.protocols import AsyncReadable
+from ophyd_async.protocols import AsyncConfigurable, AsyncReadable, AsyncStageable
 
 from .async_status import AsyncStatus
 from .device import Device
 from .signal_backend import SignalBackend
 from .sim_signal_backend import SimSignalBackend
 from .utils import DEFAULT_TIMEOUT, Callback, ReadingValueCallback, T
 
@@ -124,15 +134,15 @@
         return self._staged or bool(self._listeners)
 
     def set_staged(self, staged: bool):
         self._staged = staged
         return self._staged or bool(self._listeners)
 
 
-class SignalR(Signal[T], AsyncReadable, Stageable, Subscribable):
+class SignalR(Signal[T], AsyncReadable, AsyncStageable, Subscribable):
     """Signal that can be read from and monitored"""
 
     _cache: Optional[_SignalCache] = None
 
     def _backend_or_cache(
         self, cached: Optional[bool]
     ) -> Union[_SignalCache, SignalBackend]:
@@ -157,17 +167,17 @@
 
     @_add_timeout
     async def read(self, cached: Optional[bool] = None) -> Dict[str, Reading]:
         """Return a single item dict with the reading in it"""
         return {self.name: await self._backend_or_cache(cached).get_reading()}
 
     @_add_timeout
-    async def describe(self) -> Dict[str, Descriptor]:
+    async def describe(self) -> Dict[str, DataKey]:
         """Return a single item dict with the descriptor in it"""
-        return {self.name: await self._backend.get_descriptor(self.source)}
+        return {self.name: await self._backend.get_datakey(self.source)}
 
     @_add_timeout
     async def get_value(self, cached: Optional[bool] = None) -> T:
         """The current value"""
         return await self._backend_or_cache(cached).get_value()
 
     def subscribe_value(self, function: Callback[T]):
@@ -268,14 +278,99 @@
     soft_signal_rw if you want a device that is externally modifiable
     """
     backend = SimSignalBackend(datatype, initial_value)
     signal = SignalR(backend, name=name)
     return (signal, backend)
 
 
+async def assert_value(signal: SignalR[T], value: Any) -> None:
+    """Assert a signal's value and compare it an expected signal.
+
+    Parameters
+    ----------
+    signal:
+        signal with get_value.
+    value:
+        The expected value from the signal.
+
+    Notes
+    -----
+    Example usage::
+        await assert_value(signal, value)
+
+    """
+    assert await signal.get_value() == value
+
+
+async def assert_reading(
+    readable: AsyncReadable, reading: Mapping[str, Reading]
+) -> None:
+    """Assert readings from readable.
+
+    Parameters
+    ----------
+    readable:
+        Callable with readable.read function that generate readings.
+
+    reading:
+        The expected readings from the readable.
+
+    Notes
+    -----
+    Example usage::
+        await assert_reading(readable, reading)
+
+    """
+    assert await readable.read() == reading
+
+
+async def assert_configuration(
+    configurable: AsyncConfigurable,
+    configuration: Mapping[str, Reading],
+) -> None:
+    """Assert readings from Configurable.
+
+    Parameters
+    ----------
+    configurable:
+        Configurable with Configurable.read function that generate readings.
+
+    configuration:
+        The expected readings from configurable.
+
+    Notes
+    -----
+    Example usage::
+        await assert_configuration(configurable configuration)
+
+    """
+    assert await configurable.read_configuration() == configuration
+
+
+def assert_emitted(docs: Mapping[str, list[dict]], **numbers: int):
+    """Assert emitted document generated by running a Bluesky plan
+
+    Parameters
+    ----------
+    Doc:
+        A dictionary
+
+    numbers:
+        expected emission in kwarg from
+
+    Notes
+    -----
+    Example usage::
+        assert_emitted(docs, start=1, descriptor=1,
+        resource=1, datum=1, event=1, stop=1)
+    """
+    assert list(docs) == list(numbers)
+    assert {name: len(d) for name, d in docs.items()} == numbers
+
+
 async def observe_value(signal: SignalR[T], timeout=None) -> AsyncGenerator[T, None]:
     """Subscribe to the value of a signal so it can be iterated from.
 
     Parameters
     ----------
     signal:
         Call subscribe_value on this at the start, and clear_sub on it at the
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/signal_backend.py` & `ophyd_async-0.3a3/src/ophyd_async/core/signal_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from typing import Generic, Optional, Type
 
-from bluesky.protocols import Descriptor, Reading
+from bluesky.protocols import DataKey, Reading
 
 from .utils import DEFAULT_TIMEOUT, ReadingValueCallback, T
 
 
 class SignalBackend(Generic[T]):
     """A read/write/monitor backend for a Signals"""
 
@@ -23,15 +23,15 @@
         """Connect to underlying hardware"""
 
     @abstractmethod
     async def put(self, value: Optional[T], wait=True, timeout=None):
         """Put a value to the PV, if wait then wait for completion for up to timeout"""
 
     @abstractmethod
-    async def get_descriptor(self, source: str) -> Descriptor:
+    async def get_datakey(self, source: str) -> DataKey:
         """Metadata like source, dtype, shape, precision, units"""
 
     @abstractmethod
     async def get_reading(self) -> Reading:
         """The current value, timestamp and severity"""
 
     @abstractmethod
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/sim_signal_backend.py` & `ophyd_async-0.3a3/src/ophyd_async/core/sim_signal_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 from collections import abc
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, Generic, Optional, Type, Union, cast, get_origin
 
 import numpy as np
-from bluesky.protocols import Descriptor, Dtype, Reading
+from bluesky.protocols import DataKey, Dtype, Reading
 
 from .signal_backend import SignalBackend
 from .utils import DEFAULT_TIMEOUT, ReadingValueCallback, T, get_dtype
 
 primitive_dtypes: Dict[type, Dtype] = {
     str: "string",
     int: "integer",
@@ -32,15 +32,15 @@
     def reading(self, value: T, timestamp: float, severity: int) -> Reading:
         return Reading(
             value=value,
             timestamp=timestamp,
             alarm_severity=-1 if severity > 2 else severity,
         )
 
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         dtype = type(value)
         if np.issubdtype(dtype, np.integer):
             dtype = int
         elif np.issubdtype(dtype, np.floating):
             dtype = float
         assert (
             dtype in primitive_dtypes
@@ -52,15 +52,15 @@
         if datatype is None:
             return cast(T, None)
 
         return datatype()
 
 
 class SimArrayConverter(SimConverter):
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         return {"source": source, "dtype": "array", "shape": [len(value)]}
 
     def make_initial_value(self, datatype: Optional[Type[T]]) -> T:
         if datatype is None:
             return cast(T, None)
 
         if get_origin(datatype) == abc.Sequence:
@@ -75,15 +75,15 @@
 
     def write_value(self, value: Union[Enum, str]) -> Enum:
         if isinstance(value, Enum):
             return value
         else:
             return self.enum_class(value)
 
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         choices = [e.value for e in self.enum_class]
         return {"source": source, "dtype": "string", "shape": [], "choices": choices}  # type: ignore
 
     def make_initial_value(self, datatype: Optional[Type[T]]) -> T:
         if datatype is None:
             return cast(T, None)
 
@@ -160,16 +160,16 @@
         reading: Reading = self.converter.reading(
             self._value, self._timestamp, self._severity
         )
 
         if self.callback:
             self.callback(reading, self._value)
 
-    async def get_descriptor(self, source: str) -> Descriptor:
-        return self.converter.descriptor(source, self._value)
+    async def get_datakey(self, source: str) -> DataKey:
+        return self.converter.get_datakey(source, self._value)
 
     async def get_reading(self) -> Reading:
         return self.converter.reading(self._value, self._timestamp, self._severity)
 
     async def get_value(self) -> T:
         return self.converter.value(self._value)
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/core/utils.py` & `ophyd_async-0.3a3/src/ophyd_async/core/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/_backend/_aioca.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/_backend/_aioca.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     CANothing,
     Subscription,
     caget,
     camonitor,
     caput,
 )
 from aioca.types import AugmentedValue, Dbr, Format
-from bluesky.protocols import Descriptor, Dtype, Reading
+from bluesky.protocols import DataKey, Dtype, Reading
 from epicscorelibs.ca import dbr
 
 from ophyd_async.core import (
     ReadingValueCallback,
     SignalBackend,
     T,
     get_dtype,
@@ -54,30 +54,30 @@
     def reading(self, value: AugmentedValue):
         return {
             "value": self.value(value),
             "timestamp": value.timestamp,
             "alarm_severity": -1 if value.severity > 2 else value.severity,
         }
 
-    def descriptor(self, source: str, value: AugmentedValue) -> Descriptor:
+    def get_datakey(self, source: str, value: AugmentedValue) -> DataKey:
         return {"source": source, "dtype": dbr_to_dtype[value.datatype], "shape": []}
 
 
 class CaLongStrConverter(CaConverter):
     def __init__(self):
         return super().__init__(dbr.DBR_CHAR_STR, dbr.DBR_CHAR_STR)
 
     def write_value(self, value: str):
         # Add a null in here as this is what the commandline caput does
         # TODO: this should be in the server so check if it can be pushed to asyn
         return value + "\0"
 
 
 class CaArrayConverter(CaConverter):
-    def descriptor(self, source: str, value: AugmentedValue) -> Descriptor:
+    def get_datakey(self, source: str, value: AugmentedValue) -> DataKey:
         return {"source": source, "dtype": "array", "shape": [len(value)]}
 
 
 @dataclass
 class CaEnumConverter(CaConverter):
     enum_class: Type[Enum]
 
@@ -86,15 +86,15 @@
             return value.value
         else:
             return value
 
     def value(self, value: AugmentedValue):
         return self.enum_class(value)
 
-    def descriptor(self, source: str, value: AugmentedValue) -> Descriptor:
+    def get_datakey(self, source: str, value: AugmentedValue) -> DataKey:
         choices = [e.value for e in self.enum_class]
         return {"source": source, "dtype": "string", "shape": [], "choices": choices}
 
 
 class DisconnectedCaConverter(CaConverter):
     def __getattribute__(self, __name: str) -> Any:
         raise NotImplementedError("No PV has been set as connect() has not been called")
@@ -214,17 +214,17 @@
         return await caget(
             self.read_pv,
             datatype=self.converter.read_dbr,
             format=format,
             timeout=None,
         )
 
-    async def get_descriptor(self, source: str) -> Descriptor:
+    async def get_datakey(self, source: str) -> DataKey:
         value = await self._caget(FORMAT_CTRL)
-        return self.converter.descriptor(source, value)
+        return self.converter.get_datakey(source, value)
 
     async def get_reading(self) -> Reading:
         value = await self._caget(FORMAT_TIME)
         return self.converter.reading(value)
 
     async def get_value(self) -> T:
         value = await self._caget(FORMAT_RAW)
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/_backend/_p4p.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/_backend/_p4p.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import atexit
 import logging
 import time
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, List, Optional, Sequence, Type, Union
 
-from bluesky.protocols import Descriptor, Dtype, Reading
+from bluesky.protocols import DataKey, Dtype, Reading
 from p4p import Value
 from p4p.client.asyncio import Context, Subscription
 
 from ophyd_async.core import (
     ReadingValueCallback,
     SignalBackend,
     T,
@@ -51,15 +51,15 @@
         sv = value["alarm"]["severity"]
         return {
             "value": self.value(value),
             "timestamp": ts["secondsPastEpoch"] + ts["nanoseconds"] * 1e-9,
             "alarm_severity": -1 if sv > 2 else sv,
         }
 
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         dtype = specifier_to_dtype[value.type().aspy("value")]
         return {"source": source, "dtype": dtype, "shape": []}
 
     def metadata_fields(self) -> List[str]:
         """
         Fields to request from PVA for metadata.
         """
@@ -69,15 +69,15 @@
         """
         Fields to request from PVA for the value.
         """
         return ["value"]
 
 
 class PvaArrayConverter(PvaConverter):
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         return {"source": source, "dtype": "array", "shape": [len(value["value"])]}
 
 
 class PvaNDArrayConverter(PvaConverter):
     def metadata_fields(self) -> List[str]:
         return super().metadata_fields() + ["dimension"]
 
@@ -92,15 +92,15 @@
         # last index changing fastest.
         return dims[::-1]
 
     def value(self, value):
         dims = self._get_dimensions(value)
         return value["value"].reshape(dims)
 
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         dims = self._get_dimensions(value)
         return {"source": source, "dtype": "array", "shape": dims}
 
     def write_value(self, value):
         # No clear use-case for writing directly to an NDArray, and some
         # complexities around flattening to 1-D - e.g. dimension-order.
         # Don't support this for now.
@@ -116,47 +116,47 @@
             return value.value
         else:
             return value
 
     def value(self, value):
         return list(self.enum_class)[value["value"]["index"]]
 
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         choices = [e.value for e in self.enum_class]
         return {"source": source, "dtype": "string", "shape": [], "choices": choices}
 
 
 class PvaEnumBoolConverter(PvaConverter):
     def value(self, value):
         return value["value"]["index"]
 
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         return {"source": source, "dtype": "integer", "shape": []}
 
 
 class PvaTableConverter(PvaConverter):
     def value(self, value):
         return value["value"].todict()
 
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         # This is wrong, but defer until we know how to actually describe a table
         return {"source": source, "dtype": "object", "shape": []}  # type: ignore
 
 
 class PvaDictConverter(PvaConverter):
     def reading(self, value):
         ts = time.time()
         value = value.todict()
         # Alarm severity is vacuously 0 for a table
         return {"value": value, "timestamp": ts, "alarm_severity": 0}
 
     def value(self, value: Value):
         return value.todict()
 
-    def descriptor(self, source: str, value) -> Descriptor:
+    def get_datakey(self, source: str, value) -> DataKey:
         raise NotImplementedError("Describing Dict signals not currently supported")
 
     def metadata_fields(self) -> List[str]:
         """
         Fields to request from PVA for metadata.
         """
         return []
@@ -212,15 +212,21 @@
     elif "NTEnum" in typeid:
         # This is an Enum
         pv_choices = get_unique(
             {k: tuple(v["value"]["choices"]) for k, v in values.items()}, "choices"
         )
         return PvaEnumConverter(get_supported_enum_class(pv, datatype, pv_choices))
     elif "NTScalar" in typeid:
-        if datatype and not issubclass(typ, datatype):
+        if (
+            datatype
+            and not issubclass(typ, datatype)
+            and not (
+                typ is float and datatype is int
+            )  # Allow float -> int since prec can be 0
+        ):
             raise TypeError(f"{pv} has type {typ.__name__} not {datatype.__name__}")
         return PvaConverter()
     elif "NTTable" in typeid:
         return PvaTableConverter()
     elif "structure" in typeid:
         return PvaDictConverter()
     else:
@@ -289,17 +295,17 @@
             logging.debug(
                 f"signal pva://{self.write_pv} timed out \
                           put value: {write_value}",
                 exc_info=True,
             )
             raise NotConnected(f"pva://{self.write_pv}") from exc
 
-    async def get_descriptor(self, source: str) -> Descriptor:
+    async def get_datakey(self, source: str) -> DataKey:
         value = await self.ctxt.get(self.read_pv)
-        return self.converter.descriptor(source, value)
+        return self.converter.get_datakey(source, value)
 
     def _pva_request_string(self, fields: List[str]) -> str:
         """
         Converts a list of requested fields into a PVA request string which can be
         passed to p4p.
         """
         return f"field({','.join(fields)})"
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/_backend/common.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/_backend/common.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/aravis.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/aravis.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,35 +19,33 @@
     """
 
     _controller: AravisController
     _writer: HDFWriter
 
     def __init__(
         self,
-        name: str,
+        prefix: str,
         directory_provider: DirectoryProvider,
-        driver: AravisDriver,
-        hdf: NDFileHDF,
+        drv_suffix="cam1:",
+        hdf_suffix="HDF1:",
+        name="",
         gpio_number: AravisController.GPIO_NUMBER = 1,
-        **scalar_sigs: str,
     ):
-        # Must be child of Detector to pick up connect()
-        self.drv = driver
-        self.hdf = hdf
+        self.drv = AravisDriver(prefix + drv_suffix)
+        self.hdf = NDFileHDF(prefix + hdf_suffix)
 
         super().__init__(
             AravisController(self.drv, gpio_number=gpio_number),
             HDFWriter(
                 self.hdf,
                 directory_provider,
                 lambda: self.name,
                 ADBaseShapeProvider(self.drv),
-                **scalar_sigs,
             ),
-            config_sigs=(self.drv.acquire_time, self.drv.acquire),
+            config_sigs=(self.drv.acquire_time,),
             name=name,
         )
 
     async def _prepare(self, value: TriggerInfo) -> None:
         await self.drv.fetch_deadtime()
         await super()._prepare(value)
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/ad_base.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/ad_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/pilatus.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/pilatus.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from typing import Optional, Sequence
-
 from bluesky.protocols import Hints
 
 from ophyd_async.core import DirectoryProvider
 from ophyd_async.core.detector import StandardDetector
-from ophyd_async.core.signal import SignalR
 from ophyd_async.epics.areadetector.controllers.pilatus_controller import (
     PilatusController,
 )
 from ophyd_async.epics.areadetector.drivers.ad_base import ADBaseShapeProvider
 from ophyd_async.epics.areadetector.drivers.pilatus_driver import PilatusDriver
 from ophyd_async.epics.areadetector.writers.hdf_writer import HDFWriter
 from ophyd_async.epics.areadetector.writers.nd_file_hdf import NDFileHDF
@@ -18,33 +15,31 @@
     """A Pilatus StandardDetector writing HDF files"""
 
     _controller: PilatusController
     _writer: HDFWriter
 
     def __init__(
         self,
-        name: str,
+        prefix: str,
         directory_provider: DirectoryProvider,
-        driver: PilatusDriver,
-        hdf: NDFileHDF,
-        config_sigs: Optional[Sequence[SignalR]] = None,
-        **scalar_sigs: str,
+        drv_suffix="cam1:",
+        hdf_suffix="HDF1:",
+        name="",
     ):
-        self.drv = driver
-        self.hdf = hdf
+        self.drv = PilatusDriver(prefix + drv_suffix)
+        self.hdf = NDFileHDF(prefix + hdf_suffix)
 
         super().__init__(
             PilatusController(self.drv),
             HDFWriter(
                 self.hdf,
                 directory_provider,
                 lambda: self.name,
                 ADBaseShapeProvider(self.drv),
-                **scalar_sigs,
             ),
-            config_sigs=config_sigs or (self.drv.acquire_time,),
+            config_sigs=(self.drv.acquire_time,),
             name=name,
         )
 
     @property
     def hints(self) -> Hints:
         return self._writer.hints
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/single_trigger_det.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/single_trigger_det.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import asyncio
 from typing import Sequence
 
 from bluesky.protocols import Triggerable
 
-from ophyd_async.core import AsyncStatus, SignalR, StandardReadable
+from ophyd_async.core import (
+    AsyncStatus,
+    ConfigSignal,
+    HintedSignal,
+    SignalR,
+    StandardReadable,
+)
 
 from .drivers.ad_base import ADBase
 from .utils import ImageMode
 from .writers.nd_plugin import NDPluginBase
 
 
 class SingleTriggerDet(StandardReadable, Triggerable):
@@ -16,20 +22,22 @@
         drv: ADBase,
         read_uncached: Sequence[SignalR] = (),
         name="",
         **plugins: NDPluginBase,
     ) -> None:
         self.drv = drv
         self.__dict__.update(plugins)
-        self.set_readable_signals(
-            # Can't subscribe to read signals as race between monitor coming back and
-            # caput callback on acquire
-            read_uncached=[self.drv.array_counter] + list(read_uncached),
-            config=[self.drv.acquire_time],
+
+        self.add_readables(
+            [self.drv.array_counter, *read_uncached],
+            wrapper=HintedSignal.uncached,
         )
+
+        self.add_readables([self.drv.acquire_time], wrapper=ConfigSignal)
+
         super().__init__(name=name)
 
     @AsyncStatus.wrap
     async def stage(self) -> None:
         await asyncio.gather(
             self.drv.image_mode.set(ImageMode.single),
             self.drv.wait_for_plugins.set(True),
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/utils.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/_hdffile.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/_hdffile.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/hdf_writer.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/hdf_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from pathlib import Path
 from typing import AsyncGenerator, AsyncIterator, Dict, List, Optional
 
-from bluesky.protocols import Descriptor, Hints, StreamAsset
+from bluesky.protocols import DataKey, Hints, StreamAsset
 
 from ophyd_async.core import (
     DEFAULT_TIMEOUT,
     AsyncStatus,
     DetectorWriter,
     DirectoryProvider,
     NameProvider,
@@ -36,26 +36,29 @@
         self._shape_provider = shape_provider
         self._scalar_datasets_paths = scalar_datasets_paths
         self._capture_status: Optional[AsyncStatus] = None
         self._datasets: List[_HDFDataset] = []
         self._file: Optional[_HDFFile] = None
         self._multiplier = 1
 
-    async def open(self, multiplier: int = 1) -> Dict[str, Descriptor]:
+    async def open(self, multiplier: int = 1) -> Dict[str, DataKey]:
         self._file = None
         info = self._directory_provider()
         await asyncio.gather(
             self.hdf.num_extra_dims.set(0),
             self.hdf.lazy_open.set(True),
             self.hdf.swmr_mode.set(True),
             # See https://github.com/bluesky/ophyd-async/issues/122
             self.hdf.file_path.set(str(info.root / info.resource_dir)),
             self.hdf.file_name.set(f"{info.prefix}{self.hdf.name}{info.suffix}"),
             self.hdf.file_template.set("%s/%s.h5"),
             self.hdf.file_write_mode.set(FileWriteMode.stream),
+            # Never use custom xml layout file but use the one defined
+            # in the source code file NDFileHDF5LayoutXML.cpp
+            self.hdf.xml_file_name.set(""),
         )
 
         assert (
             await self.hdf.file_path_exists.get_value()
         ), f"File path {self.hdf.file_path.get_value()} for hdf plugin does not exist"
 
         # Overwrite num_capture to go forever
@@ -77,15 +80,15 @@
                     f"{name}-{ds_name}",
                     f"/entry/instrument/NDAttributes/{ds_path}",
                     (),
                     multiplier,
                 )
             )
         describe = {
-            ds.name: Descriptor(
+            ds.name: DataKey(
                 source=self.hdf.full_file_name.source,
                 shape=outer_shape + tuple(ds.shape),
                 dtype="array" if ds.shape else "number",
                 external="STREAM:",
             )
             for ds in self._datasets
         }
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,8 +32,9 @@
         self.num_captured = ad_r(int, prefix + "NumCaptured")
         self.swmr_mode = ad_rw(bool, prefix + "SWMRMode")
         self.lazy_open = ad_rw(bool, prefix + "LazyOpen")
         self.capture = ad_rw(bool, prefix + "Capture")
         self.flush_now = epics_signal_rw(bool, prefix + "FlushNow")
         self.array_size0 = ad_r(int, prefix + "ArraySize0")
         self.array_size1 = ad_r(int, prefix + "ArraySize1")
+        self.xml_file_name = ad_rw(str, prefix + "XMLFileName")
         super().__init__(prefix, name)
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/nd_plugin.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/nd_plugin.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/demo/__init__.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/demo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 from typing import Callable, List, Optional
 
 import numpy as np
 from bluesky.protocols import Movable, Stoppable
 
 from ophyd_async.core import (
     AsyncStatus,
+    ConfigSignal,
     Device,
     DeviceVector,
+    HintedSignal,
     StandardReadable,
     observe_value,
 )
 
 from ..signal.signal import epics_signal_r, epics_signal_rw, epics_signal_x
 
 
@@ -35,56 +37,51 @@
 
 
 class Sensor(StandardReadable):
     """A demo sensor that produces a scalar value based on X and Y Movers"""
 
     def __init__(self, prefix: str, name="") -> None:
         # Define some signals
-        self.value = epics_signal_r(float, prefix + "Value")
-        self.mode = epics_signal_rw(EnergyMode, prefix + "Mode")
-        # Set name and signals for read() and read_configuration()
-        self.set_readable_signals(
-            read=[self.value],
-            config=[self.mode],
-        )
+        with self.add_children_as_readables(HintedSignal):
+            self.value = epics_signal_r(float, prefix + "Value")
+        with self.add_children_as_readables(ConfigSignal):
+            self.mode = epics_signal_rw(EnergyMode, prefix + "Mode")
+
         super().__init__(name=name)
 
 
 class SensorGroup(StandardReadable):
     def __init__(self, prefix: str, name: str = "", sensor_count: int = 3) -> None:
-        self.sensors = DeviceVector(
-            {i: Sensor(f"{prefix}{i}:") for i in range(1, sensor_count + 1)}
-        )
-
-        # Makes read() produce the values of all sensors
-        self.set_readable_signals(
-            read=[sensor.value for sensor in self.sensors.values()],
-        )
+        with self.add_children_as_readables():
+            self.sensors = DeviceVector(
+                {i: Sensor(f"{prefix}{i}:") for i in range(1, sensor_count + 1)}
+            )
+
         super().__init__(name)
 
 
 class Mover(StandardReadable, Movable, Stoppable):
     """A demo movable that moves based on velocity"""
 
     def __init__(self, prefix: str, name="") -> None:
         # Define some signals
+        with self.add_children_as_readables(HintedSignal):
+            self.readback = epics_signal_r(float, prefix + "Readback")
+
+        with self.add_children_as_readables(ConfigSignal):
+            self.velocity = epics_signal_rw(float, prefix + "Velocity")
+            self.units = epics_signal_r(str, prefix + "Readback.EGU")
+
         self.setpoint = epics_signal_rw(float, prefix + "Setpoint")
-        self.readback = epics_signal_r(float, prefix + "Readback")
-        self.velocity = epics_signal_rw(float, prefix + "Velocity")
-        self.units = epics_signal_r(str, prefix + "Readback.EGU")
         self.precision = epics_signal_r(int, prefix + "Readback.PREC")
         # Signals that collide with standard methods should have a trailing underscore
         self.stop_ = epics_signal_x(prefix + "Stop.PROC")
         # Whether set() should complete successfully or not
         self._set_success = True
-        # Set name and signals for read() and read_configuration()
-        self.set_readable_signals(
-            read=[self.readback],
-            config=[self.velocity, self.units],
-        )
+
         super().__init__(name=name)
 
     def set_name(self, name: str):
         super().set_name(name)
         # Readback should be named the same as its parent in read()
         self.readback.set_name(name)
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/demo/demo_ad_sim_detector.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/demo/demo_ad_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/demo/mover.db` & `ophyd_async-0.3a3/src/ophyd_async/epics/demo/mover.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/demo/sensor.db` & `ophyd_async-0.3a3/src/ophyd_async/epics/demo/sensor.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/motion/motor.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/motion/motor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 import asyncio
 import time
 from typing import Callable, List, Optional
 
 from bluesky.protocols import Movable, Stoppable
 
-from ophyd_async.core import AsyncStatus, StandardReadable
+from ophyd_async.core import AsyncStatus, ConfigSignal, HintedSignal, StandardReadable
 
 from ..signal.signal import epics_signal_r, epics_signal_rw, epics_signal_x
 
 
 class Motor(StandardReadable, Movable, Stoppable):
     """Device that moves a motor record"""
 
     def __init__(self, prefix: str, name="") -> None:
         # Define some signals
+        with self.add_children_as_readables(ConfigSignal):
+            self.motor_egu = epics_signal_r(str, prefix + ".EGU")
+            self.velocity = epics_signal_rw(float, prefix + ".VELO")
+
+        with self.add_children_as_readables(HintedSignal):
+            self.user_readback = epics_signal_r(float, prefix + ".RBV")
+
         self.user_setpoint = epics_signal_rw(float, prefix + ".VAL")
-        self.user_readback = epics_signal_r(float, prefix + ".RBV")
-        self.velocity = epics_signal_rw(float, prefix + ".VELO")
         self.max_velocity = epics_signal_r(float, prefix + ".VMAX")
         self.acceleration_time = epics_signal_rw(float, prefix + ".ACCL")
-        self.motor_egu = epics_signal_r(str, prefix + ".EGU")
         self.precision = epics_signal_r(int, prefix + ".PREC")
         self.deadband = epics_signal_r(float, prefix + ".RDBD")
-        self.motor_done_move = epics_signal_r(float, prefix + ".DMOV")
-        self.low_limit_travel = epics_signal_rw(int, prefix + ".LLM")
-        self.high_limit_travel = epics_signal_rw(int, prefix + ".HLM")
+        self.motor_done_move = epics_signal_r(int, prefix + ".DMOV")
+        self.low_limit_travel = epics_signal_rw(float, prefix + ".LLM")
+        self.high_limit_travel = epics_signal_rw(float, prefix + ".HLM")
 
         self.motor_stop = epics_signal_x(prefix + ".STOP")
         # Whether set() should complete successfully or not
         self._set_success = True
-        # Set name and signals for read() and read_configuration()
-        self.set_readable_signals(
-            read=[self.user_readback],
-            config=[self.velocity, self.motor_egu],
-        )
         super().__init__(name=name)
 
     def set_name(self, name: str):
         super().set_name(name)
         # Readback should be named the same as its parent in read()
         self.user_readback.set_name(name)
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/pvi/pvi.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/pvi/pvi.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/signal/_epics_transport.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/signal/_epics_transport.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/epics/signal/signal.py` & `ophyd_async-0.3a3/src/ophyd_async/epics/signal/signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     return epics_signal_rw(datatype, f"{write_pv}{read_suffix}", write_pv, name)
 
 
 def epics_signal_r(datatype: Type[T], read_pv: str, name: str = "") -> SignalR[T]:
     """Create a `SignalR` backed by 1 EPICS PV
 
     Parameters
-    ---------
+    ----------
     datatype
         Check that the PV is of this type
     read_pv:
         The PV to read and monitor
     """
     backend = _make_backend(datatype, read_pv, read_pv)
     return SignalR(backend, name=name)
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/panda/__init__.py` & `ophyd_async-0.3a3/src/ophyd_async/panda/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/panda/_common_blocks.py` & `ophyd_async-0.3a3/src/ophyd_async/panda/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/panda/_hdf_panda.py` & `ophyd_async-0.3a3/src/ophyd_async/panda/_hdf_panda.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/panda/_panda_controller.py` & `ophyd_async-0.3a3/src/ophyd_async/panda/_panda_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/panda/_table.py` & `ophyd_async-0.3a3/src/ophyd_async/panda/_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/panda/_trigger.py` & `ophyd_async-0.3a3/src/ophyd_async/panda/_trigger.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/panda/writers/_hdf_writer.py` & `ophyd_async-0.3a3/src/ophyd_async/panda/writers/_hdf_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Any, AsyncGenerator, AsyncIterator, Dict, List, Optional
 
-from bluesky.protocols import Descriptor, StreamAsset
+from bluesky.protocols import DataKey, StreamAsset
 from p4p.client.thread import Context
 
 from ophyd_async.core import (
     DEFAULT_TIMEOUT,
     DetectorWriter,
     Device,
     DirectoryProvider,
@@ -103,15 +103,15 @@
         self._directory_provider = directory_provider
         self._name_provider = name_provider
         self._datasets: List[_HDFDataset] = []
         self._file: Optional[_HDFFile] = None
         self._multiplier = 1
 
     # Triggered on PCAP arm
-    async def open(self, multiplier: int = 1) -> Dict[str, Descriptor]:
+    async def open(self, multiplier: int = 1) -> Dict[str, DataKey]:
         """Retrieve and get descriptor of all PandA signals marked for capture"""
 
         # Get capture PVs by looking at panda. Gives mapping of dotted attribute path
         # to Signal object
         self.capture_signals = get_capture_signals(self.panda_device)
 
         # Ensure flushes are immediate
@@ -158,15 +158,15 @@
                         f"{block_name}-{signal_name}".upper() + f"-{suffix}",
                         [1],
                         multiplier=1,
                     )
                 )
 
         describe = {
-            ds.name: Descriptor(
+            ds.name: DataKey(
                 source=self.panda_device.data.hdf_directory.source,
                 shape=ds.shape,
                 dtype="array" if ds.shape != [1] else "number",
                 external="STREAM:",
             )
             for ds in self._datasets
         }
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/panda/writers/_panda_hdf_file.py` & `ophyd_async-0.3a3/src/ophyd_async/panda/writers/_panda_hdf_file.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/planstubs/prepare_trigger_and_dets.py` & `ophyd_async-0.3a3/src/ophyd_async/planstubs/prepare_trigger_and_dets.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/sim/demo/sim_motor.py` & `ophyd_async-0.3a3/src/ophyd_async/sim/demo/sim_motor.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,40 +3,42 @@
 from typing import Callable, List, Optional
 
 from bluesky.protocols import Movable, Stoppable
 
 from ophyd_async.core import StandardReadable
 from ophyd_async.core.async_status import AsyncStatus
 from ophyd_async.core.signal import soft_signal_r_and_backend, soft_signal_rw
+from ophyd_async.core.standard_readable import ConfigSignal, HintedSignal
 
 
 class SimMotor(StandardReadable, Movable, Stoppable):
     def __init__(self, name="", instant=True) -> None:
         """
         Simulated motor device
 
         args:
         - prefix: str: Signal names prefix
         - name: str: name of device
         - instant: bool: whether to move instantly, or with a delay
         """
+        with self.add_children_as_readables(HintedSignal):
+            self.user_readback, self._user_readback = soft_signal_r_and_backend(
+                float, 0
+            )
+
+        with self.add_children_as_readables(ConfigSignal):
+            self.velocity = soft_signal_rw(float, 1.0)
+            self.egu = soft_signal_rw(float, "mm")
+
         self._instant = instant
         self._move_task: Optional[asyncio.Task] = None
 
         # Define some signals
         self.user_setpoint = soft_signal_rw(float, 0)
-        self.user_readback, self._user_readback = soft_signal_r_and_backend(float, 0)
-        self.velocity = soft_signal_rw(float, 1.0)
-        self.egu = soft_signal_rw(float, "mm")
-
-        # Set name and signals for read() and read_configuration()
-        self.set_readable_signals(
-            read=[self.user_readback],
-            config=[self.velocity, self.egu],
-        )
+
         super().__init__(name=name)
 
         # Whether set() should complete successfully or not
         self._set_success = True
 
     def stop(self, success=False):
         """
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/sim/pattern_generator.py` & `ophyd_async-0.3a3/src/ophyd_async/sim/pattern_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     List,
     Optional,
     Sequence,
 )
 
 import h5py
 import numpy as np
-from bluesky.protocols import Descriptor, StreamAsset
+from bluesky.protocols import DataKey, StreamAsset
 from event_model import (
     ComposeStreamResource,
     ComposeStreamResourceBundle,
     StreamDatum,
     StreamRange,
     StreamResource,
 )
@@ -48,20 +48,20 @@
     dtype: Optional[Any] = None
     fillvalue: Optional[int] = None
 
 
 def get_full_file_description(
     datasets: List[DatasetConfig], outer_shape: tuple[int, ...]
 ):
-    full_file_description: Dict[str, Descriptor] = {}
+    full_file_description: Dict[str, DataKey] = {}
     for d in datasets:
         source = f"soft://{d.name}"
         shape = outer_shape + tuple(d.shape)
         dtype = "number" if d.shape == [1] else "array"
-        descriptor = Descriptor(
+        descriptor = DataKey(
             source=source, shape=shape, dtype=dtype, external="STREAM:"
         )
         key = d.name.replace("/", "_")
         full_file_description[key] = descriptor
     return full_file_description
 
 
@@ -215,15 +215,15 @@
         self.x = value
 
     def set_y(self, value: float) -> None:
         self.y = value
 
     async def open_file(
         self, directory: DirectoryProvider, multiplier: int = 1
-    ) -> Dict[str, Descriptor]:
+    ) -> Dict[str, DataKey]:
         await self.sim_signal.connect()
 
         self.target_path = self._get_new_path(directory)
 
         self._handle_for_h5_file = h5py.File(self.target_path, "w", libver="latest")
 
         assert self._handle_for_h5_file, "not loaded the file right"
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/sim/sim_pattern_detector_control.py` & `ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_detector_control.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/src/ophyd_async/sim/sim_pattern_detector_writer.py` & `ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_detector_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import AsyncGenerator, AsyncIterator, Dict
 
-from bluesky.protocols import Descriptor
+from bluesky.protocols import DataKey
 
 from ophyd_async.core import DirectoryProvider
 from ophyd_async.core.detector import DetectorWriter
 from ophyd_async.sim.pattern_generator import PatternGenerator
 
 
 class SimPatternDetectorWriter(DetectorWriter):
@@ -12,15 +12,15 @@
 
     def __init__(
         self, pattern_generator: PatternGenerator, directoryProvider: DirectoryProvider
     ) -> None:
         self.pattern_generator = pattern_generator
         self.directory_provider = directoryProvider
 
-    async def open(self, multiplier: int = 1) -> Dict[str, Descriptor]:
+    async def open(self, multiplier: int = 1) -> Dict[str, DataKey]:
         return await self.pattern_generator.open_file(
             self.directory_provider, multiplier
         )
 
     async def close(self) -> None:
         self.pattern_generator.close()
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async/sim/sim_pattern_generator.py` & `ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pathlib import Path
 from typing import Sequence
 
 from ophyd_async.core import DirectoryProvider, StaticDirectoryProvider
 from ophyd_async.core.detector import StandardDetector
-from ophyd_async.core.signal import SignalR
+from ophyd_async.protocols import AsyncReadable
 from ophyd_async.sim.pattern_generator import PatternGenerator
 
 from .sim_pattern_detector_control import SimPatternDetectorControl
 from .sim_pattern_detector_writer import SimPatternDetectorWriter
 
 
 class SimPatternDetector(StandardDetector):
     def __init__(
         self,
         path: Path,
-        config_sigs: Sequence[SignalR] = [],
+        config_sigs: Sequence[AsyncReadable] = [],
         name: str = "sim_pattern_detector",
         writer_timeout: float = 1,
     ) -> None:
         self.directory_provider: DirectoryProvider = StaticDirectoryProvider(path)
         self.pattern_generator = PatternGenerator()
         writer = SimPatternDetectorWriter(
             pattern_generator=self.pattern_generator,
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async.egg-info/PKG-INFO` & `ophyd_async-0.3a3/src/ophyd_async.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a2
+Version: 0.3a3
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
@@ -68,40 +68,57 @@
 Requires-Dist: numpydoc; extra == "dev"
 Requires-Dist: ophyd; extra == "dev"
 Requires-Dist: pickleshare; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: pyepics>=3.4.2; extra == "dev"
-Requires-Dist: pyside6==6.6.2; extra == "dev"
+Requires-Dist: pyside6==6.7.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-faulthandler; extra == "dev"
 Requires-Dist: pytest-rerunfailures; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
+Requires-Dist: sphinxcontrib-mermaid; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
+Requires-Dist: colorlog; extra == "dev"
 
 [![CI](https://github.com/bluesky/ophyd-async/actions/workflows/ci.yml/badge.svg)](https://github.com/bluesky/ophyd-async/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/bluesky/ophyd-async/branch/main/graph/badge.svg)](https://codecov.io/gh/bluesky/ophyd-async)
 [![PyPI](https://img.shields.io/pypi/v/ophyd-async.svg)](https://pypi.org/project/ophyd-async)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-# ophyd_async
+# ophyd-async
 
 Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 
 |    Source     |     <https://github.com/bluesky/ophyd-async>      |
 | :-----------: | :-----------------------------------------------: |
 |     PyPI      |             `pip install ophyd-async`             |
 | Documentation |      <https://bluesky.github.io/ophyd-async>      |
 |   Releases    | <https://github.com/bluesky/ophyd-async/releases> |
 
+Ophyd-async is a Python library for asynchronously interfacing with hardware, intended to 
+be used as an abstraction layer that enables experiment orchestration and data acquisition code to operate above the specifics of particular devices and control
+systems.
+
+Both ophyd and ophyd-async are typically used with the [Bluesky Run Engine][] for experiment orchestration and data acquisition.
+
+While [EPICS][] is the most common control system layer that ophyd-async can interface with, support for other control systems like [Tango][] will be supported in the future. The focus of ophyd-async is:
+
+* Asynchronous signal access, opening the possibility for hardware-triggered scanning (also known as fly-scanning)
+* Simpler instantiation of devices (groupings of signals) with less reliance upon complex class hierarchies
+
+[Bluesky Run Engine]: http://blueskyproject.io/bluesky
+[EPICS]: http://www.aps.anl.gov/epics/
+[Tango]: https://www.tango-controls.org/
+
 <!-- README only content. Anything below this line won't be included in index.md -->
 
 See https://bluesky.github.io/ophyd-async for more detailed documentation.
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async.egg-info/SOURCES.txt` & `ophyd_async-0.3a3/src/ophyd_async.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,36 +30,45 @@
 docs/index.md
 docs/reference.md
 docs/tutorials.md
 docs/_templates/README
 docs/_templates/custom-class-template.rst
 docs/_templates/custom-module-template.rst
 docs/examples/epics_demo.py
+docs/examples/foo_detector.py
 docs/explanations/decisions.md
+docs/explanations/design-goals.rst
 docs/explanations/event-loop-choice.rst
+docs/explanations/flyscanning.rst
 docs/explanations/decisions/0001-record-architecture-decisions.md
 docs/explanations/decisions/0002-switched-to-python-copier-template.md
 docs/explanations/decisions/0003-ophyd-async-migration.rst
 docs/explanations/decisions/0004-repository-structure.rst
 docs/explanations/decisions/0005-respect-black-line-length.rst
 docs/explanations/decisions/0006-procedural-device-definitions.rst
 docs/explanations/decisions/COPYME
+docs/how-to/choose-interfaces-for-devices.md
 docs/how-to/compound-devices.rst
 docs/how-to/contribute.md
 docs/how-to/make-a-simple-device.rst
+docs/how-to/make-a-standard-detector.rst
 docs/how-to/write-tests-for-devices.rst
 docs/images/bluesky_ophyd_epics_devices_logo.svg
 docs/images/bluesky_ophyd_logo.svg
+docs/images/hardware-triggered-scan.png
 docs/images/ophyd_favicon.svg
+docs/images/outer-scan.png
+docs/images/simple-hardware-scan.png
 docs/reference/api.rst
 docs/tutorials/installation.md
 docs/tutorials/using-existing-devices.rst
 src/ophyd_async/__init__.py
 src/ophyd_async/__main__.py
 src/ophyd_async/_version.py
+src/ophyd_async/log.py
 src/ophyd_async/protocols.py
 src/ophyd_async.egg-info/PKG-INFO
 src/ophyd_async.egg-info/SOURCES.txt
 src/ophyd_async.egg-info/dependency_links.txt
 src/ophyd_async.egg-info/entry_points.txt
 src/ophyd_async.egg-info/requires.txt
 src/ophyd_async.egg-info/top_level.txt
@@ -78,25 +87,31 @@
 src/ophyd_async/epics/__init__.py
 src/ophyd_async/epics/_backend/__init__.py
 src/ophyd_async/epics/_backend/_aioca.py
 src/ophyd_async/epics/_backend/_p4p.py
 src/ophyd_async/epics/_backend/common.py
 src/ophyd_async/epics/areadetector/__init__.py
 src/ophyd_async/epics/areadetector/aravis.py
+src/ophyd_async/epics/areadetector/kinetix.py
 src/ophyd_async/epics/areadetector/pilatus.py
 src/ophyd_async/epics/areadetector/single_trigger_det.py
 src/ophyd_async/epics/areadetector/utils.py
+src/ophyd_async/epics/areadetector/vimba.py
 src/ophyd_async/epics/areadetector/controllers/__init__.py
 src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
 src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
+src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
 src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
+src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
 src/ophyd_async/epics/areadetector/drivers/__init__.py
 src/ophyd_async/epics/areadetector/drivers/ad_base.py
 src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
+src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
 src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
+src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
 src/ophyd_async/epics/areadetector/writers/__init__.py
 src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
 src/ophyd_async/epics/areadetector/writers/_hdffile.py
 src/ophyd_async/epics/areadetector/writers/hdf_writer.py
 src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
 src/ophyd_async/epics/areadetector/writers/nd_plugin.py
 src/ophyd_async/epics/demo/__init__.py
@@ -128,34 +143,38 @@
 src/ophyd_async/sim/sim_pattern_detector_writer.py
 src/ophyd_async/sim/sim_pattern_generator.py
 src/ophyd_async/sim/demo/__init__.py
 src/ophyd_async/sim/demo/sim_motor.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_flyer_with_panda.py
+tests/test_log.py
 tests/core/test_async_status.py
 tests/core/test_device.py
 tests/core/test_device_collector.py
 tests/core/test_device_save_loader.py
 tests/core/test_flyer.py
 tests/core/test_signal.py
 tests/core/test_sim.py
+tests/core/test_standard_readable.py
 tests/core/test_utils.py
 tests/epics/test_pvi.py
 tests/epics/test_records.db
 tests/epics/test_signals.py
 tests/epics/_backend/test_common.py
 tests/epics/areadetector/__init__.py
 tests/epics/areadetector/test_aravis.py
 tests/epics/areadetector/test_controllers.py
 tests/epics/areadetector/test_drivers.py
+tests/epics/areadetector/test_kinetix.py
 tests/epics/areadetector/test_pilatus.py
 tests/epics/areadetector/test_scans.py
 tests/epics/areadetector/test_single_trigger_det.py
 tests/epics/areadetector/test_utils.py
+tests/epics/areadetector/test_vimba.py
 tests/epics/areadetector/test_writers.py
 tests/epics/demo/test_demo.py
 tests/epics/demo/test_demo_ad_sim_detector.py
 tests/epics/motion/__init__.py
 tests/epics/motion/test_motor.py
 tests/panda/test_hdf_panda.py
 tests/panda/test_panda_connect.py
```

### Comparing `ophyd_async-0.3a2/src/ophyd_async.egg-info/requires.txt` & `ophyd_async-0.3a3/src/ophyd_async.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -26,24 +26,26 @@
 numpydoc
 ophyd
 pickleshare
 pipdeptree
 pre-commit
 pydata-sphinx-theme>=0.12
 pyepics>=3.4.2
-pyside6==6.6.2
+pyside6==6.7.0
 pytest
 pytest-asyncio
 pytest-cov
 pytest-faulthandler
 pytest-rerunfailures
 pytest-timeout
 ruff
 sphinx-autobuild
+sphinxcontrib-mermaid
 sphinx-copybutton
 sphinx-design
 tox-direct
 types-mock
 types-pyyaml
+colorlog
 
 [pva]
 p4p
```

### Comparing `ophyd_async-0.3a2/tests/conftest.py` & `ophyd_async-0.3a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/core/test_async_status.py` & `ophyd_async-0.3a3/tests/core/test_async_status.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/core/test_device.py` & `ophyd_async-0.3a3/tests/core/test_device.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/core/test_device_collector.py` & `ophyd_async-0.3a3/tests/core/test_device_collector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/core/test_device_save_loader.py` & `ophyd_async-0.3a3/tests/core/test_device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/core/test_flyer.py` & `ophyd_async-0.3a3/tests/core/test_flyer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from enum import Enum
 from typing import Any, AsyncGenerator, AsyncIterator, Dict, Optional, Sequence
 from unittest.mock import Mock
 
 import bluesky.plan_stubs as bps
 import pytest
-from bluesky.protocols import Descriptor, StreamAsset
+from bluesky.protocols import DataKey, StreamAsset
 from bluesky.run_engine import RunEngine
 from event_model import ComposeStreamResourceBundle, compose_stream_resource
 
 from ophyd_async.core import (
     DEFAULT_TIMEOUT,
     DetectorControl,
     DetectorTrigger,
@@ -54,17 +54,17 @@
         self.dummy_signal = SignalRW(backend=SimSignalBackend(int))
         self._shape = shape
         self._name = name
         self._file: Optional[ComposeStreamResourceBundle] = None
         self._last_emitted = 0
         self.index = 0
 
-    async def open(self, multiplier: int = 1) -> Dict[str, Descriptor]:
+    async def open(self, multiplier: int = 1) -> Dict[str, DataKey]:
         return {
-            self._name: Descriptor(
+            self._name: DataKey(
                 source="soft://some-source",
                 shape=self._shape,
                 dtype="number",
                 external="STREAM:",
             )
         }
```

### Comparing `ophyd_async-0.3a2/tests/core/test_sim.py` & `ophyd_async-0.3a3/tests/core/test_sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     await backend.connect()
     q = MonitorQueue(backend)
     try:
         # Check descriptor
         source = "soft://test"
         assert dict(
             source=source, **descriptor(initial_value)
-        ) == await backend.get_descriptor(source)
+        ) == await backend.get_datakey(source)
         # Check initial value
         await q.assert_updates(
             pytest.approx(initial_value) if initial_value != "" else initial_value
         )
         # Put to new value and check that
         await backend.put(put_value)
         await q.assert_updates(pytest.approx(put_value))
@@ -133,8 +133,8 @@
         def __init__(self) -> None:
             pass
 
     sim_signal = Signal(SimSignalBackend(myClass))
     await sim_signal.connect(sim=True)
 
     with pytest.raises(AssertionError):
-        await sim_signal._backend.get_descriptor("")
+        await sim_signal._backend.get_datakey("")
```

### Comparing `ophyd_async-0.3a2/tests/core/test_utils.py` & `ophyd_async-0.3a3/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/_backend/test_common.py` & `ophyd_async-0.3a3/tests/epics/_backend/test_common.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/areadetector/test_aravis.py` & `ophyd_async-0.3a3/tests/epics/areadetector/test_aravis.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,23 @@
     DetectorTrigger,
     DeviceCollector,
     DirectoryProvider,
     TriggerInfo,
     set_sim_value,
 )
 from ophyd_async.epics.areadetector.aravis import AravisDetector
-from ophyd_async.epics.areadetector.drivers.aravis_driver import AravisDriver
-from ophyd_async.epics.areadetector.writers.nd_file_hdf import NDFileHDF
-
-
-@pytest.fixture
-async def adaravis_driver(RE: RunEngine) -> AravisDriver:
-    async with DeviceCollector(sim=True):
-        driver = AravisDriver("DRV:")
-
-    return driver
-
-
-@pytest.fixture
-async def hdf(RE: RunEngine) -> NDFileHDF:
-    async with DeviceCollector(sim=True):
-        hdf = NDFileHDF("HDF:")
-
-    return hdf
 
 
 @pytest.fixture
 async def adaravis(
     RE: RunEngine,
     static_directory_provider: DirectoryProvider,
-    adaravis_driver: AravisDriver,
-    hdf: NDFileHDF,
 ) -> AravisDetector:
     async with DeviceCollector(sim=True):
-        adaravis = AravisDetector(
-            "adaravis",
-            static_directory_provider,
-            driver=adaravis_driver,
-            hdf=hdf,
-        )
+        adaravis = AravisDetector("ADARAVIS:", static_directory_provider)
 
     return adaravis
 
 
 @pytest.mark.parametrize(
     "model,pixel_format,deadtime",
     [
```

### Comparing `ophyd_async-0.3a2/tests/epics/areadetector/test_controllers.py` & `ophyd_async-0.3a3/tests/epics/areadetector/test_controllers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/areadetector/test_drivers.py` & `ophyd_async-0.3a3/tests/epics/areadetector/test_drivers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/areadetector/test_pilatus.py` & `ophyd_async-0.3a3/tests/epics/areadetector/test_pilatus.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,72 +4,33 @@
 from ophyd_async.core import (
     DetectorTrigger,
     DeviceCollector,
     DirectoryProvider,
     TriggerInfo,
     set_sim_value,
 )
-from ophyd_async.epics.areadetector.controllers.pilatus_controller import (
-    PilatusController,
-)
-from ophyd_async.epics.areadetector.drivers.pilatus_driver import (
-    PilatusDriver,
-    PilatusTriggerMode,
-)
+from ophyd_async.epics.areadetector.drivers.pilatus_driver import PilatusTriggerMode
 from ophyd_async.epics.areadetector.pilatus import PilatusDetector
-from ophyd_async.epics.areadetector.writers.nd_file_hdf import NDFileHDF
-
-
-@pytest.fixture
-async def pilatus_driver(RE: RunEngine) -> PilatusDriver:
-    async with DeviceCollector(sim=True):
-        driver = PilatusDriver("DRV:")
-
-    return driver
-
-
-@pytest.fixture
-async def pilatus_controller(
-    RE: RunEngine, pilatus_driver: PilatusDriver
-) -> PilatusController:
-    async with DeviceCollector(sim=True):
-        controller = PilatusController(pilatus_driver)
-
-    return controller
-
-
-@pytest.fixture
-async def hdf(RE: RunEngine) -> NDFileHDF:
-    async with DeviceCollector(sim=True):
-        hdf = NDFileHDF("HDF:")
-
-    return hdf
 
 
 @pytest.fixture
 async def pilatus(
     RE: RunEngine,
     static_directory_provider: DirectoryProvider,
-    pilatus_driver: PilatusDriver,
-    hdf: NDFileHDF,
 ) -> PilatusDetector:
     async with DeviceCollector(sim=True):
-        pilatus = PilatusDetector(
-            "pilatus",
-            static_directory_provider,
-            driver=pilatus_driver,
-            hdf=hdf,
-        )
+        adpilatus = PilatusDetector("PILATUS:", static_directory_provider)
 
-    return pilatus
+    return adpilatus
 
 
 async def test_deadtime_invariant(
-    pilatus_controller: PilatusController,
+    pilatus: PilatusDetector,
 ):
+    pilatus_controller = pilatus.controller
     # deadtime invariant with exposure time
     assert pilatus_controller.get_deadtime(0) == 2.28e-3
     assert pilatus_controller.get_deadtime(500) == 2.28e-3
 
 
 @pytest.mark.parametrize(
     "detector_trigger,expected_trigger_mode",
@@ -95,15 +56,15 @@
     await trigger_and_complete()
 
     # TriggerSource changes
     assert (await pilatus.drv.trigger_mode.get_value()) == expected_trigger_mode
 
 
 async def test_hints_from_hdf_writer(pilatus: PilatusDetector):
-    assert pilatus.hints == {"fields": ["pilatus"]}
+    assert pilatus.hints == {"fields": ["adpilatus"]}
 
 
 async def test_unsupported_trigger_excepts(pilatus: PilatusDetector):
     with pytest.raises(
         ValueError,
         # str(EnumClass.value) handling changed in Python 3.11
         match=r"PilatusController only supports the following trigger types: .* but",
```

### Comparing `ophyd_async-0.3a2/tests/epics/areadetector/test_scans.py` & `ophyd_async-0.3a3/tests/epics/areadetector/test_scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/areadetector/test_single_trigger_det.py` & `ophyd_async-0.3a3/tests/epics/areadetector/test_single_trigger_det.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/areadetector/test_utils.py` & `ophyd_async-0.3a3/tests/epics/areadetector/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/areadetector/test_writers.py` & `ophyd_async-0.3a3/tests/epics/areadetector/test_writers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/demo/test_demo.py` & `ophyd_async-0.3a3/tests/epics/demo/test_demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import asyncio
 import subprocess
+from collections import defaultdict
 from typing import Dict
 from unittest.mock import ANY, Mock, call, patch
 
 import pytest
+from bluesky import plans as bp
 from bluesky.protocols import Reading
+from bluesky.run_engine import RunEngine
 
 from ophyd_async.core import (
     DeviceCollector,
     NotConnected,
+    assert_emitted,
+    assert_reading,
+    assert_value,
     set_sim_callback,
     set_sim_value,
 )
 from ophyd_async.epics import demo
 
 # Long enough for multiple asyncio event loop cycles to run so
 # all the tasks have a chance to run
@@ -80,15 +86,16 @@
         current=0.0,
         initial=0.0,
         target=0.55,
         unit="mm",
         precision=3,
         time_elapsed=pytest.approx(0.0, abs=0.05),
     )
-    assert 0.55 == await sim_mover.setpoint.get_value()
+
+    await assert_value(sim_mover.setpoint, 0.55)
     assert not s.done
     done.assert_not_called()
     await asyncio.sleep(0.1)
     set_sim_value(sim_mover.readback, 0.1)
     await watcher.wait_for_call(
         name="sim_mover",
         current=0.1,
@@ -106,32 +113,38 @@
     done2 = Mock()
     s.add_callback(done2)
     done2.assert_called_once_with(s)
 
 
 async def test_sensor_reading_shows_value(sim_sensor: demo.Sensor):
     # Check default value
+    await assert_value(sim_sensor.value, pytest.approx(0.0))
     assert (await sim_sensor.value.get_value()) == pytest.approx(0.0)
-    assert (await sim_sensor.read()) == {
-        "sim_sensor-value": {
-            "alarm_severity": 0,
-            "timestamp": ANY,
-            "value": 0.0,
-        }
-    }
-
+    await assert_reading(
+        sim_sensor,
+        {
+            "sim_sensor-value": {
+                "value": 0.0,
+                "alarm_severity": 0,
+                "timestamp": ANY,
+            }
+        },
+    )
     # Check different value
     set_sim_value(sim_sensor.value, 5.0)
-    assert (await sim_sensor.read()) == {
-        "sim_sensor-value": {
-            "alarm_severity": 0,
-            "timestamp": ANY,
-            "value": 5.0,
-        }
-    }
+    await assert_reading(
+        sim_sensor,
+        {
+            "sim_sensor-value": {
+                "value": 5.0,
+                "timestamp": ANY,
+                "alarm_severity": 0,
+            }
+        },
+    )
 
 
 async def test_mover_stopped(sim_mover: demo.Mover):
     callbacks = []
     set_sim_callback(sim_mover.stop_, lambda r, v: callbacks.append(v))
 
     assert callbacks == [None]
@@ -198,14 +211,29 @@
     set_sim_value(sim_sensor.mode, demo.EnergyMode.high)
     assert (await sim_sensor.read_configuration())["sim_sensor-mode"][
         "value"
     ] == demo.EnergyMode.high
     await sim_sensor.unstage()
 
 
+async def test_sensor_in_plan(RE: RunEngine, sim_sensor: demo.Sensor):
+    """Tests sim sensor behavior within a RunEngine plan.
+
+    This test verifies that the sensor emits the expected documents
+     when used in plan(count).
+    """
+    docs = defaultdict(list)
+
+    def capture_emitted(name, doc):
+        docs[name].append(doc)
+
+    RE(bp.count([sim_sensor], num=2), capture_emitted)
+    assert_emitted(docs, start=1, descriptor=1, event=2, stop=1)
+
+
 async def test_assembly_renaming() -> None:
     thing = demo.SampleStage("PRE")
     await thing.connect(sim=True)
     assert thing.x.name == ""
     assert thing.x.velocity.name == ""
     assert thing.x.stop_.name == ""
     await thing.x.velocity.set(456)
@@ -241,17 +269,36 @@
 ):
     set_sim_value(sim_sensor_group.sensors[1].value, 0.0)
     set_sim_value(sim_sensor_group.sensors[2].value, 0.5)
     set_sim_value(sim_sensor_group.sensors[3].value, 1.0)
 
     await sim_sensor_group.stage()
     description = await sim_sensor_group.describe()
-    reading = await sim_sensor_group.read()
-    await sim_sensor_group.unstage()
 
+    await sim_sensor_group.unstage()
+    await assert_reading(
+        sim_sensor_group,
+        {
+            "sim_sensor_group-sensors-1-value": {
+                "value": 0.0,
+                "timestamp": ANY,
+                "alarm_severity": 0,
+            },
+            "sim_sensor_group-sensors-2-value": {
+                "value": 0.5,
+                "timestamp": ANY,
+                "alarm_severity": 0,
+            },
+            "sim_sensor_group-sensors-3-value": {
+                "value": 1.0,
+                "timestamp": ANY,
+                "alarm_severity": 0,
+            },
+        },
+    )
     assert description == {
         "sim_sensor_group-sensors-1-value": {
             "dtype": "number",
             "shape": [],
             "source": "soft://sim_sensor_group-sensors-1-value",
         },
         "sim_sensor_group-sensors-2-value": {
@@ -261,31 +308,14 @@
         },
         "sim_sensor_group-sensors-3-value": {
             "dtype": "number",
             "shape": [],
             "source": "soft://sim_sensor_group-sensors-3-value",
         },
     }
-    assert reading == {
-        "sim_sensor_group-sensors-1-value": {
-            "alarm_severity": 0,
-            "timestamp": ANY,
-            "value": 0.0,
-        },
-        "sim_sensor_group-sensors-2-value": {
-            "alarm_severity": 0,
-            "timestamp": ANY,
-            "value": 0.5,
-        },
-        "sim_sensor_group-sensors-3-value": {
-            "alarm_severity": 0,
-            "timestamp": ANY,
-            "value": 1.0,
-        },
-    }
 
 
 @patch("ophyd_async.epics.demo.subprocess.Popen")
 async def test_ioc_starts(mock_popen: Mock):
     demo.start_ioc_subprocess()
     mock_popen.assert_called_once_with(
         ANY,
```

### Comparing `ophyd_async-0.3a2/tests/epics/demo/test_demo_ad_sim_detector.py` & `ophyd_async-0.3a3/tests/epics/demo/test_demo_ad_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/motion/test_motor.py` & `ophyd_async-0.3a3/tests/epics/motion/test_motor.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/test_pvi.py` & `ophyd_async-0.3a3/tests/epics/test_pvi.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/test_records.db` & `ophyd_async-0.3a3/tests/epics/test_records.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/epics/test_signals.py` & `ophyd_async-0.3a3/tests/epics/test_signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,17 +129,15 @@
 ):
     backend = await ioc.make_backend(datatype, suffix)
     # Make a monitor queue that will monitor for updates
     q = MonitorQueue(backend)
     try:
         # Check descriptor
         pv_name = f"{ioc.protocol}://{PV_PREFIX}:{ioc.protocol}:{suffix}"
-        assert dict(source=pv_name, **descriptor) == await backend.get_descriptor(
-            pv_name
-        )
+        assert dict(source=pv_name, **descriptor) == await backend.get_datakey(pv_name)
         # Check initial value
         await q.assert_updates(pytest.approx(initial_value))
         # Put to new value and check that
         await backend.put(put_value)
         await q.assert_updates(pytest.approx(put_value))
     finally:
         q.close()
@@ -405,15 +403,15 @@
     # Make and connect the backend
     for t, i, p in [(MyTable, initial, put), (None, put, initial)]:
         backend = await ioc.make_backend(t, "table")
         # Make a monitor queue that will monitor for updates
         q = MonitorQueue(backend)
         try:
             # Check descriptor
-            dict(source="test-source", **descriptor) == await backend.get_descriptor(
+            dict(source="test-source", **descriptor) == await backend.get_datakey(
                 "test-source"
             )
             # Check initial value
             await q.assert_updates(approx_table(i))
             # Put to new value and check that
             await backend.put(p)
             await q.assert_updates(approx_table(p))
@@ -442,15 +440,15 @@
         },
         "record": ANY,
     }
 
     try:
         # Check descriptor
         with pytest.raises(NotImplementedError):
-            await backend.get_descriptor("")
+            await backend.get_datakey("")
         # Check initial value
         await q.assert_updates(expected)
         await backend.get_value()
 
     finally:
         q.close()
 
@@ -472,15 +470,15 @@
     # Make a monitor queue that will monitor for updates
     for i, p in [(initial, put), (put, initial)]:
         with closing(MonitorQueue(backend)) as q:
             assert {
                 "source": "test-source",
                 "dtype": "array",
                 "shape": [2, 3],
-            } == await backend.get_descriptor("test-source")
+            } == await backend.get_datakey("test-source")
             # Check initial value
             await q.assert_updates(pytest.approx(i))
             await raw_data_backend.put(p.flatten())
             await q.assert_updates(pytest.approx(p))
 
 
 async def test_writing_to_ndarray_raises_typeerror(ioc: IOC):
```

### Comparing `ophyd_async-0.3a2/tests/panda/db/panda.db` & `ophyd_async-0.3a3/tests/panda/db/panda.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/panda/test_hdf_panda.py` & `ophyd_async-0.3a3/tests/panda/test_hdf_panda.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,25 @@
 from bluesky.run_engine import RunEngine
 
 from ophyd_async.core import StaticDirectoryProvider, set_sim_value
 from ophyd_async.core.async_status import AsyncStatus
 from ophyd_async.core.detector import DetectorControl, DetectorTrigger
 from ophyd_async.core.device import Device
 from ophyd_async.core.flyer import HardwareTriggeredFlyable
-from ophyd_async.core.signal import SignalR, wait_for_value
+from ophyd_async.core.signal import SignalR, assert_emitted, wait_for_value
 from ophyd_async.core.sim_signal_backend import SimSignalBackend
 from ophyd_async.core.utils import DEFAULT_TIMEOUT
 from ophyd_async.panda import HDFPanda, PcapBlock
 from ophyd_async.panda._trigger import StaticSeqTableTriggerLogic
 from ophyd_async.panda.writers._hdf_writer import Capture
 from ophyd_async.planstubs.prepare_trigger_and_dets import (
     prepare_static_seq_table_flyer_and_detectors_with_same_trigger,
 )
 
 
-def assert_emitted(docs: Dict[str, list], **numbers: int):
-    assert list(docs) == list(numbers)
-    assert {name: len(d) for name, d in docs.items()} == numbers
-
-
 class MockPandaPcapController(DetectorControl):
     def __init__(self, pcap: PcapBlock) -> None:
         self.pcap = pcap
 
     def get_deadtime(self, exposure: float) -> float:
         return 0.000000008
```

### Comparing `ophyd_async-0.3a2/tests/panda/test_panda_connect.py` & `ophyd_async-0.3a3/tests/panda/test_panda_connect.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/panda/test_panda_controller.py` & `ophyd_async-0.3a3/tests/panda/test_panda_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/panda/test_panda_utils.py` & `ophyd_async-0.3a3/tests/panda/test_panda_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/panda/test_table.py` & `ophyd_async-0.3a3/tests/panda/test_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/panda/test_trigger.py` & `ophyd_async-0.3a3/tests/panda/test_trigger.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/panda/test_writer.py` & `ophyd_async-0.3a3/tests/panda/test_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/protocols/test_protocols.py` & `ophyd_async-0.3a3/tests/protocols/test_protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/sim/test_pattern_generator.py` & `ophyd_async-0.3a3/tests/sim/test_pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/sim/test_sim_detector.py` & `ophyd_async-0.3a3/tests/sim/test_sim_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     assert sim_pattern_detector.controller
 
 
 async def test_writes_pattern_to_file(
     sim_pattern_detector: SimPatternDetector, sim_motor: motor.Motor, tmp_path
 ):
     sim_pattern_detector = SimPatternDetector(
-        config_sigs=[*sim_motor._read_signals], path=tmp_path
+        config_sigs=[*sim_motor._readables], path=tmp_path
     )
 
     images_number = 2
     await sim_pattern_detector.controller.arm(num=images_number)
     # assert that the file is created and non-empty
     assert sim_pattern_detector.writer
```

### Comparing `ophyd_async-0.3a2/tests/sim/test_sim_writer.py` & `ophyd_async-0.3a3/tests/sim/test_sim_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a2/tests/sim/test_streaming_plan.py` & `ophyd_async-0.3a3/tests/sim/test_streaming_plan.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from collections import defaultdict
-from typing import Dict
 
 from bluesky import plans as bp
 from bluesky.run_engine import RunEngine
 
+from ophyd_async.core.signal import assert_emitted
 from ophyd_async.sim.sim_pattern_generator import SimPatternDetector
 
 
-def assert_emitted(docs: Dict[str, list], **numbers: int):
-    assert list(docs) == list(numbers)
-    assert {name: len(d) for name, d in docs.items()} == numbers
-
-
 # NOTE the async operations with h5py are non-trival
 # because of lack of native support for async operations
 # see https://github.com/h5py/h5py/issues/837
 async def test_streaming_plan(RE: RunEngine, sim_pattern_detector: SimPatternDetector):
     names = []
     docs = []
```

### Comparing `ophyd_async-0.3a2/tests/test_flyer_with_panda.py` & `ophyd_async-0.3a3/tests/test_flyer_with_panda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from typing import AsyncGenerator, AsyncIterator, Dict, Optional, Sequence
 from unittest.mock import Mock
 
 import bluesky.plan_stubs as bps
 import pytest
-from bluesky.protocols import Descriptor, StreamAsset
+from bluesky.protocols import DataKey, StreamAsset
 from bluesky.run_engine import RunEngine
 from event_model import ComposeStreamResourceBundle, compose_stream_resource
 
 from ophyd_async.core import (
     DEFAULT_TIMEOUT,
     DetectorControl,
     DetectorWriter,
@@ -32,17 +32,17 @@
         self.dummy_signal = SignalRW(backend=SimSignalBackend(int))
         self._shape = shape
         self._name = name
         self._file: Optional[ComposeStreamResourceBundle] = None
         self._last_emitted = 0
         self.index = 0
 
-    async def open(self, multiplier: int = 1) -> Dict[str, Descriptor]:
+    async def open(self, multiplier: int = 1) -> Dict[str, DataKey]:
         return {
-            self._name: Descriptor(
+            self._name: DataKey(
                 source="soft://some-source",
                 shape=self._shape,
                 dtype="number",
                 external="STREAM:",
             )
         }
```

