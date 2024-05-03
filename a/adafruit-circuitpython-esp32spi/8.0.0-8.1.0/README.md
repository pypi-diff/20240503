# Comparing `tmp/adafruit_circuitpython_esp32spi-8.0.0.tar.gz` & `tmp/adafruit_circuitpython_esp32spi-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_esp32spi-8.0.0.tar", last modified: Tue Apr 30 15:56:38 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_esp32spi-8.1.0.tar", last modified: Fri May  3 02:15:49 2024, max compression
```

## Comparing `adafruit_circuitpython_esp32spi-8.0.0.tar` & `adafruit_circuitpython_esp32spi-8.1.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.780486 adafruit_circuitpython_esp32spi-8.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.768486 adafruit_circuitpython_esp32spi-8.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.768486 adafruit_circuitpython_esp32spi-8.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.772486 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.772486 adafruit_circuitpython_esp32spi-8.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 15:56:38.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.772486 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3180 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/PWMOut.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38979 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6293 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/digitalio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_ipconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_localtime.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_settings.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_simpletest_rp2040.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_tcp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_udp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_wpa2ent_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_wpa2ent_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/esp32spi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/gpio.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:38.776486 adafruit_circuitpython_esp32spi-8.0.0/examples/server/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/examples/server/esp32spi_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 15:56:36.000000 adafruit_circuitpython_esp32spi-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 15:56:29.000000 adafruit_circuitpython_esp32spi-8.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:56:38.780486 adafruit_circuitpython_esp32spi-8.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.488589 adafruit_circuitpython_esp32spi-8.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.492589 adafruit_circuitpython_esp32spi-8.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.492589 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.492589 adafruit_circuitpython_esp32spi-8.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.496589 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3180 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/PWMOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39665 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6293 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/digitalio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.496589 adafruit_circuitpython_esp32spi-8.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.496589 adafruit_circuitpython_esp32spi-8.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_ipconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_settings.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_simpletest_rp2040.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_tcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_wpa2ent_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_wpa2ent_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/esp32spi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/gpio.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/examples/server/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/server/esp32spi_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/setup.cfg
```

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_esp32spi-8.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/.gitignore` & `adafruit_circuitpython_esp32spi-8.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/.pre-commit-config.yaml` & `adafruit_circuitpython_esp32spi-8.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/.pylintrc` & `adafruit_circuitpython_esp32spi-8.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_esp32spi-8.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/LICENSE` & `adafruit_circuitpython_esp32spi-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_esp32spi-8.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/LICENSES/MIT.txt` & `adafruit_circuitpython_esp32spi-8.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_esp32spi-8.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/PKG-INFO` & `adafruit_circuitpython_esp32spi-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 8.0.0
+Version: 8.1.0
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/README.rst` & `adafruit_circuitpython_esp32spi-8.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO` & `adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 8.0.0
+Version: 8.1.0
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt` & `adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/PWMOut.py` & `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/PWMOut.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi.py` & `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import struct
 import time
 from micropython import const
 from adafruit_bus_device.spi_device import SPIDevice
 from digitalio import Direction
 
-__version__ = "8.0.0"
+__version__ = "8.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI.git"
 
 _SET_NET_CMD = const(0x10)
 _SET_PASSPHRASE_CMD = const(0x11)
 _SET_IP_CONFIG = const(0x14)
 _SET_DNS_CONFIG = const(0x15)
 _SET_HOSTNAME = const(0x16)
@@ -368,20 +368,20 @@
             print("MAC address")
         resp = self._send_command_get_response(_GET_MACADDR_CMD, [b"\xFF"])
         return resp[0]
 
     @property
     def MAC_address_actual(self):  # pylint: disable=invalid-name
         """A bytearray containing the actual MAC address of the ESP32"""
-        if self._debug:
-            print("MAC address")
-        resp = self._send_command_get_response(_GET_MACADDR_CMD, [b"\xFF"])
-        new_resp = bytearray(resp[0])
-        new_resp = reversed(new_resp)
-        return new_resp
+        return bytearray(reversed(self.MAC_address))
+
+    @property
+    def mac_address(self):
+        """A bytes containing the actual MAC address of the ESP32"""
+        return bytes(self.MAC_address_actual)
 
     def start_scan_networks(self):
         """Begin a scan of visible access points. Follow up with a call
         to 'get_scan_networks' for response"""
         if self._debug:
             print("Start scan")
         resp = self._send_command_get_response(_START_SCAN_NETWORKS)
@@ -541,41 +541,53 @@
 
     @property
     def ip_address(self):
         """Our local IP address"""
         return self.network_data["ip_addr"]
 
     @property
-    def is_connected(self):
+    def connected(self):
         """Whether the ESP32 is connected to an access point"""
         try:
             return self.status == WL_CONNECTED
         except OSError:
             self.reset()
             return False
 
     @property
+    def is_connected(self):
+        """Whether the ESP32 is connected to an access point"""
+        return self.connected
+
+    @property
     def ap_listening(self):
         """Returns if the ESP32 is in access point mode and is listening for connections"""
         try:
             return self.status == WL_AP_LISTENING
         except OSError:
             self.reset()
             return False
 
     def disconnect(self):
         """Disconnect from the access point"""
         resp = self._send_command_get_response(_DISCONNECT_CMD)
         if resp[0][0] != 1:
             raise OSError("Failed to disconnect")
 
-    def connect(self, secrets):
-        """Connect to an access point using a secrets dictionary
-        that contains a 'ssid' and 'password' entry"""
-        self.connect_AP(secrets["ssid"], secrets["password"])
+    def connect(self, ssid, password=None, timeout=10):
+        """Connect to an access point with given name and password.
+
+        **Deprecated functionality:** If the first argument (``ssid``) is a ``dict``,
+        assume it is a dictionary with entries for keys ``"ssid"`` and, optionally, ``"password"``.
+        This mimics the previous signature for ``connect()``.
+        This upward compatbility will be removed in a future release.
+        """
+        if isinstance(ssid, dict):  # secrets
+            ssid, password = ssid["ssid"], ssid.get("password")
+        self.connect_AP(ssid, password, timeout_s=timeout)
 
     def connect_AP(self, ssid, password, timeout_s=10):  # pylint: disable=invalid-name
         """Connect to an access point with given name and password.
         Will wait until specified timeout seconds and return on success
         or raise an exception on failure.
 
         :param ssid: the SSID to connect to
@@ -643,14 +655,19 @@
             if stat == WL_AP_LISTENING:
                 return stat
             time.sleep(0.05)
         if stat == WL_AP_FAILED:
             raise ConnectionError("Failed to create AP", ssid)
         raise OSError("Unknown error 0x%02x" % stat)
 
+    @property
+    def ipv4_address(self):
+        """IP address of the station when connected to an access point."""
+        return self.pretty_ip(self.ip_address)
+
     def pretty_ip(self, ip):  # pylint: disable=no-self-use, invalid-name
         """Converts a bytearray IP address to a dotted-quad string for printing"""
         return "%d.%d.%d.%d" % (ip[0], ip[1], ip[2], ip[3])
 
     def unpretty_ip(self, ip):  # pylint: disable=no-self-use, invalid-name
         """Converts a dotted-quad string to a bytearray IP address"""
         octets = [int(x) for x in ip.split(".")]
```

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py` & `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py` & `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/adafruit_esp32spi/digitalio.py` & `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/digitalio.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/docs/_static/favicon.ico` & `adafruit_circuitpython_esp32spi-8.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/docs/api.rst` & `adafruit_circuitpython_esp32spi-8.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/docs/conf.py` & `adafruit_circuitpython_esp32spi-8.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/docs/index.rst` & `adafruit_circuitpython_esp32spi-8.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_aio_post.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_cheerlights.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_ipconfig.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_ipconfig.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_localtime.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_localtime.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_settings.toml` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_settings.toml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_simpletest.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_simpletest_rp2040.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_simpletest_rp2040.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_tcp_client.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_tcp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_udp_client.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_udp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_wpa2ent_aio_post.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_wpa2ent_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/esp32spi_wpa2ent_simpletest.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_wpa2ent_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/esp32spi_gpio.py` & `adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/esp32spi_gpio.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/examples/gpio/gpio.md` & `adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/gpio.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.0.0/pyproject.toml` & `adafruit_circuitpython_esp32spi-8.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-esp32spi"
 description = "CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI"
-version = "8.0.0"
+version = "8.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI"}
 keywords = [
     "adafruit",
```

