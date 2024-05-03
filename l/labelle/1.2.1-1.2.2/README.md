# Comparing `tmp/labelle-1.2.1.tar.gz` & `tmp/labelle-1.2.2.tar.gz`

## Comparing `labelle-1.2.1.tar` & `labelle-1.2.2.tar`

### file list

```diff
@@ -1,89 +1,93 @@
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 labelle-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 labelle-1.2.1/labelle.ini
--rw-r--r--   0        0        0   635825 2020-02-02 00:00:00.000000 labelle-1.2.1/labelle.png
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 labelle-1.2.1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 labelle-1.2.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 labelle-1.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 labelle-1.2.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 labelle-1.2.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 labelle-1.2.1/.vscode/launch.json
--rw-r--r--   0        0        0    43688 2020-02-02 00:00:00.000000 labelle-1.2.1/doc/Labelle_example_1.png
--rw-r--r--   0        0        0    41426 2020-02-02 00:00:00.000000 labelle-1.2.1/doc/Labelle_example_2.png
--rw-r--r--   0        0        0    50874 2020-02-02 00:00:00.000000 labelle-1.2.1/doc/Labelle_example_3.png
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 labelle-1.2.1/scripts/gui_dev.sh
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_version.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/metadata.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib.pyi
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE
--rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_AMSFONTS
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_BAKOMA
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_CARLOGO
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_COLORBREWER
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_COURIERTEN
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_DEJAVU
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_JSXTOOLS_RESIZE_OBSERVER
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_QHULL
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_QT4_EDITOR
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_SOLARIZED
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_STIX
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_YORICK
--rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/_vendor/matplotlib/font_manager.py
--rwxr-xr-x   0        0        0    11632 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/cli/cli.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/gui/common.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/gui/gui.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/gui/q_actions.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/gui/q_device_selector.py
--rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/gui/q_label_widgets.py
--rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/gui/q_labels_list.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/gui/q_render.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/gui/q_settings_toolbar.py
--rwxr-xr-x   0        0        0     4017 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/barcode_writer.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/config_file.py
--rwxr-xr-x   0        0        0     3102 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/constants.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/env_config.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/font_config.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/logger.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/outputs.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/unicode_blocks.py
--rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/devices/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/devices/device_manager.py
--rwxr-xr-x   0        0        0    12025 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/devices/dymo_labeler.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/devices/online_device_manager.py
--rw-r--r--   0        0        0     9909 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/devices/usb_device.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/__init__.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/barcode.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/barcode_with_text.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/empty.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/horizontally_combined.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/margins.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/picture.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/print_payload.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/print_preview.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/qr.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/render_context.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/render_engine.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/test_pattern.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/lib/render_engines/text.py
--rw-r--r--   0        0        0   690516 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/fonts/Carlito-Bold.ttf
--rw-r--r--   0        0        0   816716 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0        0        0   623416 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/fonts/Carlito-Italic.ttf
--rw-r--r--   0        0        0   635996 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/fonts/Carlito-Regular.ttf
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/fonts/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/fonts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/icons/__init__.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/icons/barcode_icon.png
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/icons/barcode_text_icon.png
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/icons/img_icon.png
--rw-r--r--   0        0        0    68086 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/icons/logo_small.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/icons/qr_icon.png
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 labelle-1.2.1/src/labelle/resources/icons/txt_icon.png
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 labelle-1.2.1/vendoring/README.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 labelle-1.2.1/vendoring/vendor.txt
--rw-r--r--   0        0        0    47308 2020-02-02 00:00:00.000000 labelle-1.2.1/vendoring/patches/matplotlib.patch
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 labelle-1.2.1/.gitignore
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 labelle-1.2.1/LICENSE
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 labelle-1.2.1/README.md
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 labelle-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 labelle-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 labelle-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 labelle-1.2.2/labelle.ini
+-rw-r--r--   0        0        0   635825 2020-02-02 00:00:00.000000 labelle-1.2.2/labelle.png
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 labelle-1.2.2/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 labelle-1.2.2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 labelle-1.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 labelle-1.2.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 labelle-1.2.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 labelle-1.2.2/.vscode/launch.json
+-rw-r--r--   0        0        0    43688 2020-02-02 00:00:00.000000 labelle-1.2.2/doc/Labelle_example_1.png
+-rw-r--r--   0        0        0    41426 2020-02-02 00:00:00.000000 labelle-1.2.2/doc/Labelle_example_2.png
+-rw-r--r--   0        0        0    50874 2020-02-02 00:00:00.000000 labelle-1.2.2/doc/Labelle_example_3.png
+-rw-r--r--   0        0        0    19248 2020-02-02 00:00:00.000000 labelle-1.2.2/doc/choose_a_tag.png
+-rw-r--r--   0        0        0    63146 2020-02-02 00:00:00.000000 labelle-1.2.2/doc/draft_a_new_release.png
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 labelle-1.2.2/doc/release.md
+-rw-r--r--   0        0        0    54711 2020-02-02 00:00:00.000000 labelle-1.2.2/doc/trusted_publisher_management.png
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 labelle-1.2.2/scripts/gui_dev.sh
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_version.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/metadata.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib.pyi
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_AMSFONTS
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_BAKOMA
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_CARLOGO
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_COLORBREWER
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_COURIERTEN
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_DEJAVU
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_JSXTOOLS_RESIZE_OBSERVER
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_QHULL
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_QT4_EDITOR
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_SOLARIZED
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_STIX
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_YORICK
+-rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/_vendor/matplotlib/font_manager.py
+-rwxr-xr-x   0        0        0    16652 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/cli/cli.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/gui/common.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/gui/gui.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/gui/q_actions.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/gui/q_device_selector.py
+-rw-r--r--   0        0        0    15264 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/gui/q_label_widgets.py
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/gui/q_labels_list.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/gui/q_render.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/gui/q_settings_toolbar.py
+-rwxr-xr-x   0        0        0     4017 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/barcode_writer.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/config_file.py
+-rwxr-xr-x   0        0        0     3102 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/constants.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/env_config.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/font_config.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/logger.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/outputs.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/unicode_blocks.py
+-rwxr-xr-x   0        0        0     1369 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/devices/__init__.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/devices/device_manager.py
+-rwxr-xr-x   0        0        0    12089 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/devices/dymo_labeler.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/devices/online_device_manager.py
+-rw-r--r--   0        0        0    10063 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/devices/usb_device.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/__init__.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/barcode.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/barcode_with_text.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/empty.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/horizontally_combined.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/margins.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/picture.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/print_payload.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/print_preview.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/qr.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/render_context.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/render_engine.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/test_pattern.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/lib/render_engines/text.py
+-rw-r--r--   0        0        0   690516 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/fonts/Carlito-Bold.ttf
+-rw-r--r--   0        0        0   816716 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0        0        0   623416 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/fonts/Carlito-Italic.ttf
+-rw-r--r--   0        0        0   635996 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/fonts/Carlito-Regular.ttf
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/fonts/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/fonts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/icons/__init__.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/icons/barcode_icon.png
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/icons/barcode_text_icon.png
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/icons/img_icon.png
+-rw-r--r--   0        0        0    68086 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/icons/logo_small.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/icons/qr_icon.png
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 labelle-1.2.2/src/labelle/resources/icons/txt_icon.png
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 labelle-1.2.2/vendoring/README.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 labelle-1.2.2/vendoring/vendor.txt
+-rw-r--r--   0        0        0    47308 2020-02-02 00:00:00.000000 labelle-1.2.2/vendoring/patches/matplotlib.patch
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 labelle-1.2.2/.gitignore
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 labelle-1.2.2/LICENSE
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 labelle-1.2.2/README.md
+-rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 labelle-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 labelle-1.2.2/PKG-INFO
```

### Comparing `labelle-1.2.1/.pre-commit-config.yaml` & `labelle-1.2.2/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -16,30 +16,38 @@
   - id: check-yaml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
     args: ['--fix=lf']
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.1
+  rev: v0.4.2
   hooks:
   - id: ruff
     args: [--fix, --exit-non-zero-on-fix]
   - id: ruff-format
 
 - repo: https://gitlab.com/bmares/check-json5
   rev: v1.0.0
   hooks:
   - id: check-json5
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.9.0
+  rev: v1.10.0
   hooks:
   - id: mypy
     additional_dependencies:
+    - darkdetect
+    - platformdirs
+    # This is a hack to get type checking for PyQt6 but to stay under
+    # pre-commit.ci's 250MiB limit.
+    # <https://github.com/maresb/pyqt6-without-qt>
+    - pyqt6-without-qt
+    - typer
     - types-pillow
     - types-cffi
+    - types-pygments
 
 - repo: https://github.com/igorshubovych/markdownlint-cli
   rev: v0.39.0
   hooks:
   - id: markdownlint
```

### Comparing `labelle-1.2.1/labelle.png` & `labelle-1.2.2/labelle.png`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/.devcontainer/Dockerfile` & `labelle-1.2.2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/.devcontainer/devcontainer.json` & `labelle-1.2.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/.github/workflows/pypi-publish.yml` & `labelle-1.2.2/.github/workflows/pypi-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,25 @@
       run: |
         python -m pip install --upgrade pip build twine
         python -m build
     - name: Test wheels
       run: |
         python -m twine check dist/*
     - name: Upload dist files for publication
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v4
       with:
         name: dist-files
         path: dist
   publish:
     runs-on: ubuntu-latest
     needs: build
     # Run this job in an isolated GHA environment containing the OIDC credentials.
     environment: release
     permissions:
       id-token: write
     steps:
-    - uses: actions/download-artifact@v2
+    - uses: actions/download-artifact@v4
       with:
         name: dist-files
         path: dist
     - name: Publish
       uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `labelle-1.2.1/.github/workflows/tests.yml` & `labelle-1.2.2/.github/workflows/tests.yml`

 * *Files 17% similar despite different names*

```diff
@@ -17,11 +17,12 @@
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
+        sudo apt-get install -y libegl1
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
       run: tox
```

### Comparing `labelle-1.2.1/.vscode/launch.json` & `labelle-1.2.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/doc/Labelle_example_1.png` & `labelle-1.2.2/doc/Labelle_example_1.png`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/doc/Labelle_example_2.png` & `labelle-1.2.2/doc/Labelle_example_2.png`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/doc/Labelle_example_3.png` & `labelle-1.2.2/doc/Labelle_example_3.png`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_AMSFONTS` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_AMSFONTS`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_BAKOMA` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_BAKOMA`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_CARLOGO` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_CARLOGO`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_COLORBREWER` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_COLORBREWER`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_COURIERTEN` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_COURIERTEN`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_DEJAVU` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_DEJAVU`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_JSXTOOLS_RESIZE_OBSERVER` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_JSXTOOLS_RESIZE_OBSERVER`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_QHULL` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_QHULL`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_QT4_EDITOR` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_QT4_EDITOR`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_SOLARIZED` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_SOLARIZED`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_STIX` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_STIX`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/LICENSE_YORICK` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/LICENSE_YORICK`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/_vendor/matplotlib/font_manager.py` & `labelle-1.2.2/src/labelle/_vendor/matplotlib/font_manager.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/gui/gui.py` & `labelle-1.2.2/src/labelle/gui/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class LabelleWindow(QWidget):
     _label_bitmap_to_print: Optional[Image.Image]
     _device_manager: DeviceManager
     _dymo_labeler: DymoLabeler
     _render_context: RenderContext
     _render_widget: QWidget
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self._label_bitmap_to_print = None
         self._detected_device = None
 
         self._window_layout = QVBoxLayout()
 
         self._device_selector = QDeviceSelector(self)
@@ -51,39 +51,39 @@
         self._init_layout()
 
         self._device_selector.repopulate()
         self._settings_toolbar.on_settings_changed()
         self._label_list.populate()
         self._label_list.render_label()
 
-    def _init_elements(self):
+    def _init_elements(self) -> None:
         self.setWindowTitle("Labelle GUI")
         self.setWindowIcon(QIcon(str(ICON_DIR / "logo_small.png")))
         self.setGeometry(200, 200, 1100, 400)
 
         self._device_manager = DeviceManager()
         self._dymo_labeler = DymoLabeler()
         self._settings_toolbar.update_labeler_context(
             supported_tape_sizes=self._dymo_labeler.SUPPORTED_TAPE_SIZES_MM,
             installed_tape_size=self._dymo_labeler.tape_size_mm,
             minimum_horizontal_margin_mm=self._dymo_labeler.minimum_horizontal_margin_mm,
         )
 
-    def _init_connections(self):
+    def _init_connections(self) -> None:
         self._label_list.renderPrintPreviewSignal.connect(self._update_preview_render)
         self._label_list.renderPrintPayloadSignal.connect(self._update_print_render)
         self._actions.print_label_signal.connect(self._on_print_label)
         self._settings_toolbar.settings_changed_signal.connect(
             self._on_settings_changed
         )
         self._device_selector.selectedDeviceChangedSignal.connect(
             self._on_device_selected
         )
 
-    def _init_layout(self):
+    def _init_layout(self) -> None:
         self._actions.setParent(self._render_widget)
         self._render.setParent(self._render_widget)
 
         render_layout = QHBoxLayout(self._render_widget)
         render_layout.addWidget(
             self._render, alignment=QtCore.Qt.AlignmentFlag.AlignRight
         )
@@ -93,15 +93,15 @@
 
         self._window_layout.addWidget(self._device_selector)
         self._window_layout.addWidget(self._settings_toolbar)
         self._window_layout.addWidget(self._label_list)
         self._window_layout.addWidget(self._render_widget)
         self.setLayout(self._window_layout)
 
-    def _on_settings_changed(self, settings: Settings):
+    def _on_settings_changed(self, settings: Settings) -> None:
         assert self._dymo_labeler is not None
         self._dymo_labeler.tape_size_mm = settings.tape_size_mm
 
         # Update render context
         self._render_context = RenderContext(
             foreground_color=settings.foreground_color,
             background_color=settings.background_color,
@@ -117,50 +117,50 @@
         )
 
         is_ready = self._dymo_labeler.is_ready
         self._settings_toolbar.setEnabled(is_ready)
         self._label_list.setEnabled(is_ready)
         self._render_widget.setEnabled(is_ready)
 
-    def _update_preview_render(self, preview_bitmap):
+    def _update_preview_render(self, preview_bitmap: Image.Image) -> None:
         self._render.update_preview_render(preview_bitmap)
 
-    def _update_print_render(self, label_bitmap_to_print):
+    def _update_print_render(self, label_bitmap_to_print) -> None:
         self._label_bitmap_to_print = label_bitmap_to_print
 
-    def _on_print_label(self):
+    def _on_print_label(self) -> None:
         try:
             if self._label_bitmap_to_print is None:
                 raise RuntimeError("No label to print! Call update_label_render first.")
             assert self._dymo_labeler is not None
             self._dymo_labeler.print(self._label_bitmap_to_print)
         except DymoLabelerPrintError as err:
             crash_msg_box(self, "Printing Failed!", err)
 
-    def _on_device_selected(self):
+    def _on_device_selected(self) -> None:
         self._dymo_labeler.device = self._device_selector.selected_device
         self._settings_toolbar.on_settings_changed()
 
 
-def parse(app):
+def parse(app) -> None:
     """Parse the arguments and options of the given app object."""
     parser = QCommandLineParser()
     parser.addHelpOption()
 
     verbose_option = QCommandLineOption(["v", "verbose"], "Verbose output.")
     parser.addOption(verbose_option)
     parser.process(app)
 
     is_verbose = parser.isSet(verbose_option)
     if (not is_verbose) and (not is_verbose_env_vars()):
         # Neither the --verbose flag nor the environment variable is set.
         set_not_verbose()
 
 
-def main():
+def main() -> None:
     configure_logging()
     with system_run():
         app = QApplication(sys.argv)
         parse(app)
         window = LabelleWindow()
         window.show()
         sys.exit(app.exec())
```

### Comparing `labelle-1.2.1/src/labelle/gui/q_actions.py` & `labelle-1.2.2/src/labelle/gui/q_actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,42 +24,42 @@
         self._last_error = None
         self._print_button = QPushButton()
 
         self._init_elements()
         self._init_connections()
         self._init_layout()
 
-    def _init_elements(self):
+    def _init_elements(self) -> None:
         printer_icon = QIcon.fromTheme("printer")
         self._print_button.setIcon(printer_icon)
         self._print_button.setFixedSize(64, 64)
         self._print_button.setIconSize(QSize(48, 48))
 
-    def _init_connections(self):
+    def _init_connections(self) -> None:
         self._print_button.clicked.connect(self._on_print_label)
 
-    def _init_layout(self):
+    def _init_layout(self) -> None:
         layout = QVBoxLayout(self)
         layout.addWidget(
             self._print_button, alignment=QtCore.Qt.AlignmentFlag.AlignRight
         )
         layout.addWidget(
             self._error_label, alignment=QtCore.Qt.AlignmentFlag.AlignCenter
         )
 
-    def _on_print_label(self):
+    def _on_print_label(self) -> None:
         self.print_label_signal.emit()
 
-    def clear_error(self):
+    def clear_error(self) -> None:
         self._error_label.setText("")
         self._last_error = None
         self._print_button.setEnabled(True)
         self._print_button.setCursor(Qt.CursorShape.ArrowCursor)
 
-    def set_error(self, error: str):
+    def set_error(self, error: str) -> None:
         if self._last_error == error:
             return
         self._last_error = error
         self._error_label.setText(error)
         LOG.error(error)
         self._print_button.setDisabled(True)
         self._print_button.setCursor(Qt.CursorShape.ForbiddenCursor)
```

### Comparing `labelle-1.2.1/src/labelle/gui/q_device_selector.py` & `labelle-1.2.2/src/labelle/gui/q_device_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         self._init_elements()
         self._init_connections()
         self._init_layout()
 
         self._last_scan_error_changed()
         self.selectedDeviceChangedSignal.emit()
 
-    def _init_elements(self):
+    def _init_elements(self) -> None:
         self.device_manager = OnlineDeviceManager()
 
-    def _init_connections(self):
+    def _init_connections(self) -> None:
         self.device_manager.devices_changed_signal.connect(self.repopulate)
         self.device_manager.last_scan_error_changed_signal.connect(
             self._last_scan_error_changed
         )
         self._devices.currentIndexChanged.connect(self._index_changed)
 
-    def repopulate(self):
+    def repopulate(self) -> None:
         old_hashes = {device.hash for device in self.device_manager.devices}
         self._devices.clear()
         for idx, device in enumerate(self.device_manager.devices):
             self._devices.insertItem(idx, device.product, device.hash)
             if (
                 self._selected_device is not None
                 and self._selected_device.hash == device.hash
@@ -67,27 +67,27 @@
         assert self._action_error_label is not None
         self._action_devices.setVisible(valid)
         self._action_error_label.setVisible(not valid)
         new_hashes = {device.hash for device in self.device_manager.devices}
         if new_hashes != old_hashes:
             self.selectedDeviceChangedSignal.emit()
 
-    def _index_changed(self, index):
+    def _index_changed(self, index) -> None:
         if index >= 0:
             self._selected_device = self.device_manager.devices[index]
         else:
             self._selected_device = None
         self.selectedDeviceChangedSignal.emit()
 
-    def _last_scan_error_changed(self):
+    def _last_scan_error_changed(self) -> None:
         last_scan_error = self.device_manager.last_scan_error or ""
         self._error_label.setText(str(last_scan_error))
         self.repopulate()
 
-    def _init_layout(self):
+    def _init_layout(self) -> None:
         self._devices.setSizeAdjustPolicy(QComboBox.SizeAdjustPolicy.AdjustToContents)
         self._action_devices = self.addWidget(self._devices)
         self._action_error_label = self.addWidget(self._error_label)
 
     @property
     def selected_device(self) -> UsbDevice | None:
         device = None
```

### Comparing `labelle-1.2.1/src/labelle/gui/q_label_widgets.py` & `labelle-1.2.2/src/labelle/gui/q_label_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     RenderEngine,
     TextRenderEngine,
 )
 from labelle.lib.render_engines.render_engine import RenderEngineException
 
 
 class FontStyle(QComboBox):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         # Populate font_style
         for font_path in get_available_fonts():
             name = font_path.stem
             absolute_path = font_path.absolute()
             self.addItem(name, absolute_path)
             self.setCurrentText("Carlito-Regular")
@@ -63,25 +63,25 @@
 
     """
 
     render_context: RenderContext
 
     itemRenderSignal = QtCore.pyqtSignal(name="itemRenderSignal")
 
-    def content_changed(self):
+    def content_changed(self) -> None:
         """Emit the itemRenderSignal when the content of the label is changed."""
         self.itemRenderSignal.emit()
 
     @property
-    def render_engine_impl(self):
+    def render_engine_impl(self) -> None:
         """Abstract method for getting the render engine of the label."""
         pass
 
     @property
-    def render_engine(self):
+    def render_engine(self) -> Optional[RenderEngine]:
         try:
             return self.render_engine_impl
         except RenderEngineException as err:
             crash_msg_box(self, "Render Engine Failed!", err)
             return EmptyRenderEngine()
 
 
@@ -147,15 +147,15 @@
         self.label.textChanged.connect(self.content_changed)
         self.frame_width_px.valueChanged.connect(self.content_changed)
         self.font_size.valueChanged.connect(self.content_changed)
         self.font_style.currentTextChanged.connect(self.content_changed)
         self.align.currentTextChanged.connect(self.content_changed)
         self.setLayout(layout)
 
-    def content_changed(self):
+    def content_changed(self) -> None:
         """Manage changes to the label contents.
 
         In particular, update the height of the label and emit the itemRenderSignal
         when the content of the label changes.
         """
         self.label.setFixedHeight(15 * (len(self.label.toPlainText().splitlines()) + 2))
         self.setFixedHeight(self.label.height() + 10)
@@ -353,15 +353,15 @@
                 QIcon(str(ICON_DIR / "barcode_text_icon.png")).pixmap(32, 32)
             )
         else:
             self.item_icon.setPixmap(
                 QIcon(str(ICON_DIR / "barcode_icon.png")).pixmap(32, 32)
             )
 
-    def toggle_text_fields_and_rerender(self):
+    def toggle_text_fields_and_rerender(self) -> None:
         is_checked = self.show_text_checkbox.isChecked()
         self.set_text_fields_visibility(is_checked)
         self.content_changed()  # Trigger rerender
 
     @property
     def render_engine_impl(self):
         """Get the render engine for the barcode label using the current settings.
```

### Comparing `labelle-1.2.1/src/labelle/gui/q_labels_list.py` & `labelle-1.2.2/src/labelle/gui/q_labels_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import logging
-from typing import Optional
+from typing import List, Optional
 
 from PIL import Image
 from PyQt6 import QtCore
 from PyQt6.QtGui import QAction
 from PyQt6.QtWidgets import QAbstractItemView, QListWidget, QListWidgetItem, QMenu
 
 from labelle.gui.common import crash_msg_box
 from labelle.gui.q_label_widgets import (
     BarcodeDymoLabelWidget,
+    BaseLabelWidget,
     EmptyRenderEngine,
     ImageDymoLabelWidget,
     QrDymoLabelWidget,
     TextDymoLabelWidget,
 )
 from labelle.lib.constants import Direction
 from labelle.lib.devices.dymo_labeler import DymoLabeler
 from labelle.lib.render_engines import (
     HorizontallyCombinedRenderEngine,
     PrintPayloadRenderEngine,
     PrintPreviewRenderEngine,
     RenderContext,
 )
 from labelle.lib.render_engines.render_engine import (
+    RenderEngine,
     RenderEngineException,
 )
 from labelle.lib.utils import mm_to_px
 
 LOG = logging.getLogger(__name__)
 
 
@@ -69,15 +71,14 @@
     renderPrintPreviewSignal = QtCore.pyqtSignal(
         Image.Image, name="renderPrintPreviewSignal"
     )
     renderPrintPayloadSignal = QtCore.pyqtSignal(
         Image.Image, name="renderPrintPayloadSignal"
     )
     render_context: Optional[RenderContext]
-    itemWidget: TextDymoLabelWidget
     dymo_labeler: Optional[DymoLabeler]
     h_margin_mm: float
     min_label_width_mm: Optional[float]
     justify: Direction
 
     def __init__(self, parent=None):
         super().__init__(parent)
@@ -85,15 +86,15 @@
         self.h_margin_mm = 0.0
         self.min_label_width_mm = None
         self.justify = Direction.CENTER
         self.render_context = None
         self.setAlternatingRowColors(True)
         self.setDragDropMode(QAbstractItemView.DragDropMode.InternalMove)
 
-    def populate(self):
+    def populate(self) -> None:
         assert self.render_context is not None
         for item_widget in [TextDymoLabelWidget(self.render_context)]:
             item = QListWidgetItem(self)
             item.setSizeHint(item_widget.sizeHint())
             self.addItem(item)
             self.setItemWidget(item, item_widget)
             item_widget.itemRenderSignal.connect(self.render_label)
@@ -131,29 +132,33 @@
         self.dymo_labeler = dymo_labeler
         self.h_margin_mm = h_margin_mm
         self.min_label_width_mm = min_label_width_mm
         self.justify = justify
         self.render_context = render_context
         for i in range(self.count()):
             item_widget = self.itemWidget(self.item(i))
+            assert isinstance(item_widget, BaseLabelWidget)
             item_widget.render_context = render_context
         self.render_label()
 
     @property
     def _payload_render_engine(self):
-        render_engines = []
+        render_engines: List[RenderEngine] = []
         for i in range(self.count()):
             item = self.item(i)
             item_widget = self.itemWidget(self.item(i))
             if item_widget and item:
                 item.setSizeHint(item_widget.sizeHint())
-                render_engines.append(item_widget.render_engine)
+                assert isinstance(item_widget, BaseLabelWidget)
+                render_engine = item_widget.render_engine
+                if render_engine is not None:
+                    render_engines.append(render_engine)
         return HorizontallyCombinedRenderEngine(render_engines=render_engines)
 
-    def render_preview(self):
+    def render_preview(self) -> None:
         assert self.dymo_labeler is not None
         assert self.render_context is not None
         render_engine = PrintPreviewRenderEngine(
             render_engine=self._payload_render_engine,
             justify=self.justify,
             visible_horizontal_margin_px=mm_to_px(self.h_margin_mm),
             labeler_margin_px=self.dymo_labeler.labeler_margin_px,
@@ -164,15 +169,15 @@
             bitmap = render_engine.render(self.render_context)
         except RenderEngineException as err:
             crash_msg_box(self, "Render Engine Failed!", err)
             bitmap = EmptyRenderEngine().render(self.render_context)
 
         self.renderPrintPreviewSignal.emit(bitmap)
 
-    def render_print(self):
+    def render_print(self) -> None:
         assert self.dymo_labeler is not None
         assert self.render_context is not None
         render_engine = PrintPayloadRenderEngine(
             render_engine=self._payload_render_engine,
             justify=self.justify,
             visible_horizontal_margin_px=mm_to_px(self.h_margin_mm),
             labeler_margin_px=self.dymo_labeler.labeler_margin_px,
@@ -183,19 +188,19 @@
             bitmap, _ = render_engine.render_with_meta(self.render_context)
         except RenderEngineException as err:
             crash_msg_box(self, "Render Engine Failed!", err)
             bitmap = EmptyRenderEngine().render(self.render_context)
 
         self.renderPrintPayloadSignal.emit(bitmap)
 
-    def render_label(self):
+    def render_label(self) -> None:
         self.render_preview()
         self.render_print()
 
-    def contextMenuEvent(self, event):
+    def contextMenuEvent(self, event) -> None:
         """Override the default context menu event to add or delete label widgets.
 
         Args:
         ----
             event (QContextMenuEvent): The context menu event.
 
         """
@@ -206,43 +211,43 @@
         add_barcode: Optional[QAction] = contextMenu.addAction("Add Barcode")
         add_img: Optional[QAction] = contextMenu.addAction("Add Image")
         delete: Optional[QAction] = contextMenu.addAction("Delete")
         menu_click = contextMenu.exec(event.globalPos())
 
         if menu_click == add_text:
             item = QListWidgetItem(self)
-            item_widget = TextDymoLabelWidget(self.render_context)
-            item.setSizeHint(item_widget.sizeHint())
+            text_item_widget = TextDymoLabelWidget(self.render_context)
+            item.setSizeHint(text_item_widget.sizeHint())
             self.addItem(item)
-            self.setItemWidget(item, item_widget)
-            item_widget.itemRenderSignal.connect(self.render_label)
+            self.setItemWidget(item, text_item_widget)
+            text_item_widget.itemRenderSignal.connect(self.render_label)
 
         if menu_click == add_qr:
             item = QListWidgetItem(self)
-            item_widget = QrDymoLabelWidget(self.render_context)
-            item.setSizeHint(item_widget.sizeHint())
+            qr_item_widget = QrDymoLabelWidget(self.render_context)
+            item.setSizeHint(qr_item_widget.sizeHint())
             self.addItem(item)
-            self.setItemWidget(item, item_widget)
-            item_widget.itemRenderSignal.connect(self.render_label)
+            self.setItemWidget(item, qr_item_widget)
+            qr_item_widget.itemRenderSignal.connect(self.render_label)
 
         if menu_click == add_barcode:
             item = QListWidgetItem(self)
-            item_widget = BarcodeDymoLabelWidget(self.render_context)
-            item.setSizeHint(item_widget.sizeHint())
+            barcode_item_widget = BarcodeDymoLabelWidget(self.render_context)
+            item.setSizeHint(barcode_item_widget.sizeHint())
             self.addItem(item)
-            self.setItemWidget(item, item_widget)
-            item_widget.itemRenderSignal.connect(self.render_label)
+            self.setItemWidget(item, barcode_item_widget)
+            barcode_item_widget.itemRenderSignal.connect(self.render_label)
 
         if menu_click == add_img:
             item = QListWidgetItem(self)
-            item_widget = ImageDymoLabelWidget(self.render_context)
-            item.setSizeHint(item_widget.sizeHint())
+            image_item_widget = ImageDymoLabelWidget(self.render_context)
+            item.setSizeHint(image_item_widget.sizeHint())
             self.addItem(item)
-            self.setItemWidget(item, item_widget)
-            item_widget.itemRenderSignal.connect(self.render_label)
+            self.setItemWidget(item, image_item_widget)
+            image_item_widget.itemRenderSignal.connect(self.render_label)
         if menu_click == delete:
             try:
                 item_to_delete = self.itemAt(event.pos())
                 self.takeItem(self.indexFromItem(item_to_delete).row())  # self.update()
             except Exception as e:  # noqa: BLE001
                 LOG.warning(f"No item selected {e}")
         self.render_label()
```

### Comparing `labelle-1.2.1/src/labelle/gui/q_render.py` & `labelle-1.2.2/src/labelle/gui/q_render.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 from typing import Optional
 
-from PIL import ImageQt
+from PIL import Image, ImageQt
 from PyQt6.QtGui import QPixmap
 from PyQt6.QtWidgets import QGraphicsDropShadowEffect, QLabel, QWidget
 
 LOG = logging.getLogger(__name__)
 
 
 class QRender(QLabel):
-    def __init__(self, parent: Optional[QWidget] = None):
+    def __init__(self, parent: Optional[QWidget] = None) -> None:
         super().__init__(parent)
         self._init_elements()
 
-    def _init_elements(self):
+    def _init_elements(self) -> None:
         shadow = QGraphicsDropShadowEffect()
         shadow.setBlurRadius(15)
         self.setGraphicsEffect(shadow)
 
-    def update_preview_render(self, preview_bitmap):
+    def update_preview_render(self, preview_bitmap: Image.Image) -> None:
         qim = ImageQt.ImageQt(preview_bitmap)
         q_image = QPixmap.fromImage(qim)
         self.setPixmap(q_image)
         self.adjustSize()
```

### Comparing `labelle-1.2.1/src/labelle/gui/q_settings_toolbar.py` & `labelle-1.2.2/src/labelle/gui/q_settings_toolbar.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,49 +43,49 @@
         self._tape_size_mm = QComboBox()
 
         self._init_elements()
         self._init_connections()
         self._init_layout()
         self.on_settings_changed()
 
-    def _init_elements(self):
+    def _init_elements(self) -> None:
         self._horizontal_margin_mm.setMaximum(HORIZONTAL_MARGIN_MM__MAX_VALUE)
         self._min_label_width_mm.setMaximum(MIN_LABEL_WIDTH_MM__MIN_VALUE)
         self._justify.addItems(d.value for d in Direction)
         self._foreground_color.addItems(FOREGROUND_COLOR__VALUES)
         self._background_color.addItems(BACKGROUND_COLOR__VALUES)
         self._preview_show_margins.setChecked(PREVIEW_SHOW_MARGINS__DEFAULT_VALUE)
 
     def update_labeler_context(
         self,
         supported_tape_sizes: tuple[int, ...],
         installed_tape_size: int,
         minimum_horizontal_margin_mm: float,
-    ):
+    ) -> None:
         for tape_size_mm in supported_tape_sizes:
             self._tape_size_mm.addItem(str(tape_size_mm), tape_size_mm)
         tape_size_index = supported_tape_sizes.index(installed_tape_size)
         self._tape_size_mm.setCurrentIndex(tape_size_index)
 
         h_margins_mm = round(minimum_horizontal_margin_mm)
         self._horizontal_margin_mm.setMinimum(h_margins_mm)
         if not self._horizontal_margin_mm.value():
             self._horizontal_margin_mm.setValue(h_margins_mm)
         self._min_label_width_mm.setMinimum(h_margins_mm * 2)
 
-    def _init_connections(self):
+    def _init_connections(self) -> None:
         self._background_color.currentTextChanged.connect(self.on_settings_changed)
         self._foreground_color.currentTextChanged.connect(self.on_settings_changed)
         self._horizontal_margin_mm.valueChanged.connect(self.on_settings_changed)
         self._justify.currentTextChanged.connect(self.on_settings_changed)
         self._min_label_width_mm.valueChanged.connect(self.on_settings_changed)
         self._preview_show_margins.stateChanged.connect(self.on_settings_changed)
         self._tape_size_mm.currentTextChanged.connect(self.on_settings_changed)
 
-    def _init_layout(self):
+    def _init_layout(self) -> None:
         self.addWidget(QLabel("Margin [mm]:"))
         self.addWidget(self._horizontal_margin_mm)
         self.addSeparator()
         self.addWidget(QLabel("Tape Size [mm]:"))
         self.addWidget(self._tape_size_mm)
         self.addSeparator()
         self.addWidget(QLabel("Min Label Length [mm]:"))
@@ -98,20 +98,20 @@
         self.addWidget(self._foreground_color)
         self.addWidget(QLabel(" on "))
         self.addWidget(self._background_color)
         self.addWidget(QLabel("Show margins:"))
         self.addWidget(self._preview_show_margins)
 
     @property
-    def settings(self):
+    def settings(self) -> Settings:
         return Settings(
             background_color=self._background_color.currentText(),
             foreground_color=self._foreground_color.currentText(),
             horizontal_margin_mm=self._horizontal_margin_mm.value(),
             justify=Direction(self._justify.currentText()),
             min_label_width_mm=self._min_label_width_mm.value(),
             preview_show_margins=self._preview_show_margins.isChecked(),
             tape_size_mm=self._tape_size_mm.currentData(),
         )
 
-    def on_settings_changed(self):
+    def on_settings_changed(self) -> None:
         self.settings_changed_signal.emit(self.settings)
```

### Comparing `labelle-1.2.1/src/labelle/lib/barcode_writer.py` & `labelle-1.2.2/src/labelle/lib/barcode_writer.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/config_file.py` & `labelle-1.2.2/src/labelle/lib/config_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,12 +30,12 @@
     if config_parser.read(file_to_read):
         logger.debug(f"Read config file: {file_to_read}")
     else:
         logger.debug(f"Config file not found: {file_to_read}")
     return config_parser
 
 
-def get_config_section(section_name) -> Optional[Dict[str, Any]]:
+def get_config_section(section_name: str) -> Optional[Dict[str, Any]]:
     config = get_config()
     if section_name not in config:
         return None
     return dict(config[section_name])
```

### Comparing `labelle-1.2.1/src/labelle/lib/constants.py` & `labelle-1.2.2/src/labelle/lib/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,10 +103,10 @@
     CENTER = "center"
     RIGHT = "right"
 
 
 class Output(str, Enum):
     PRINTER = "printer"
     CONSOLE = "console"
-    CONSOLE_INVERTED = "console_inverted"
+    CONSOLE_INVERTED = "console-inverted"
     BROWSER = "browser"
     IMAGEMAGICK = "imagemagick"
```

### Comparing `labelle-1.2.1/src/labelle/lib/font_config.py` & `labelle-1.2.2/src/labelle/lib/font_config.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/logger.py` & `labelle-1.2.2/src/labelle/lib/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 import sys
 
 _IS_VERBOSE = True
 LOG = logging.getLogger("labelle")
 VERBOSE_NOTICE = "Run with --verbose for more information"
 
 
-def _update_log_level():
+def _update_log_level() -> None:
     LOG.setLevel(logging.DEBUG if _IS_VERBOSE else logging.INFO)
 
 
 def set_not_verbose() -> None:
     global _IS_VERBOSE
     _IS_VERBOSE = False
     _update_log_level()
 
 
 def is_verbose() -> bool:
     return _IS_VERBOSE
 
 
-def configure_logging():
+def configure_logging() -> None:
     handler = logging.StreamHandler(sys.stderr)
     formatter = logging.Formatter("[%(levelname)s] %(message)s")
     handler.setFormatter(formatter)
 
     _update_log_level()
     LOG.addHandler(handler)
```

### Comparing `labelle-1.2.1/src/labelle/lib/outputs.py` & `labelle-1.2.2/src/labelle/lib/outputs.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/unicode_blocks.py` & `labelle-1.2.2/src/labelle/lib/unicode_blocks.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/utils.py` & `labelle-1.2.2/src/labelle/lib/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 # permitted in any medium without royalty provided the copyright notice and
 # this notice are preserved.
 # === END LICENSE STATEMENT ===
 import contextlib
 import logging
 import math
 import sys
+from typing import Generator, List, Tuple
 
 from PIL import ImageDraw
 
 from labelle.lib.constants import PIXELS_PER_MM
 from labelle.lib.logger import print_exception
 
 LOG = logging.getLogger(__name__)
 
 
-def scaling(pix, sc):
+def scaling(pix, sc) -> List[Tuple[int, int]]:
     """Scaling pixel up, input: (x,y),scale-factor."""
     return [(pix[0] + i, pix[1] + j) for i in range(sc) for j in range(sc)]
 
 
 @contextlib.contextmanager
-def draw_image(bitmap):
+def draw_image(bitmap) -> Generator[ImageDraw.ImageDraw, None, None]:
     drawobj = ImageDraw.Draw(bitmap)
     assert isinstance(drawobj, ImageDraw.ImageDraw)
     try:
         yield drawobj
     finally:
         del drawobj
 
@@ -40,13 +41,13 @@
 
 
 def mm_to_px(mm) -> float:
     return mm * PIXELS_PER_MM
 
 
 @contextlib.contextmanager
-def system_run():
+def system_run() -> Generator[None, None, None]:
     try:
         yield
     except Exception as e:  # noqa: BLE001
         print_exception(e)
         sys.exit(1)
```

### Comparing `labelle-1.2.1/src/labelle/lib/devices/device_manager.py` & `labelle-1.2.2/src/labelle/lib/devices/device_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class DeviceManagerNoDevices(DeviceManagerError):
     pass
 
 
 class DeviceManager:
     _devices: dict[str, UsbDevice]
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._devices = {}
 
     def scan(self) -> bool:
         prev = self._devices
         try:
             cur = {dev.hash: dev for dev in UsbDevice.supported_devices() if dev.hash}
         except POSSIBLE_USB_ERRORS as e:
```

### Comparing `labelle-1.2.1/src/labelle/lib/devices/dymo_labeler.py` & `labelle-1.2.2/src/labelle/lib/devices/dymo_labeler.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,30 +129,30 @@
         if not self._response:
             return None
         self._response = False
         responseBin = self._devin.read(8)
         response = array.array("B", responseBin).tolist()
         return response
 
-    def _reset_command(self):
+    def _reset_command(self) -> None:
         """Remove a partially built command (MLF)."""
         self._cmd = []
         self._response = False
 
     def _build_command(self, cmd):
         """Add the next instruction to the command (MLF)."""
         self._cmd += cmd
 
-    def _status_request(self):
+    def _status_request(self) -> None:
         """Set instruction to get the device's status (MLF)."""
         cmd = [ESC, ord("A")]
         self._build_command(cmd)
         self._response = True
 
-    def _dot_tab(self, value, tape_size_mm: int):
+    def _dot_tab(self, value, tape_size_mm: int) -> None:
         """Set the bias text height, in bytes (MLF)."""
         if value < 0 or value > self._max_bytes_per_line(tape_size_mm):
             raise ValueError
         cmd = [ESC, ord("B"), value]
         self._build_command(cmd)
         self._dotTab = value
         self._bytesPerLine = None
@@ -168,40 +168,40 @@
         """Set the number of bytes sent in the following lines (MLF)."""
         if value == self._bytesPerLine:
             return
         cmd = [ESC, ord("D"), value]
         self._build_command(cmd)
         self._bytesPerLine = value
 
-    def _cut(self):
+    def _cut(self) -> None:
         """Set instruction to trigger cutting of the tape (MLF)."""
         cmd = [ESC, ord("E")]
         self._build_command(cmd)
 
-    def _line(self, value):
+    def _line(self, value) -> None:
         """Set next printed line (MLF)."""
         self._bytes_per_line(len(value))
         cmd = [SYN, *value]
         self._build_command(cmd)
 
-    def _chain_mark(self, tape_size_mm: int):
+    def _chain_mark(self, tape_size_mm: int) -> None:
         """Set Chain Mark (MLF)."""
         self._dot_tab(0, tape_size_mm)
         self._bytes_per_line(self._max_bytes_per_line(tape_size_mm))
         self._line([0x99] * self._max_bytes_per_line(tape_size_mm))
 
-    def _skip_lines(self, value):
+    def _skip_lines(self, value) -> None:
         """Set number of lines of white to print (MLF)."""
         if value <= 0:
             raise ValueError
         self._bytes_per_line(0)
         cmd = [SYN] * value
         self._build_command(cmd)
 
-    def _init_label(self):
+    def _init_label(self) -> None:
         """Set the label initialization sequence (MLF).
 
         This was in the original dymoprint by S. Bronner but was never invoked.
         (There was a self.initLabel without parentheses.)
         I see no mention of it in the technical reference, so this seems to be
         dead code.
         """
```

### Comparing `labelle-1.2.1/src/labelle/lib/devices/online_device_manager.py` & `labelle-1.2.2/src/labelle/lib/devices/online_device_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,35 +19,35 @@
     _status_time: QTimer
     _device_manager: DeviceManager
     last_scan_error_changed_signal = QtCore.pyqtSignal(
         name="lastScanErrorChangedSignal"
     )
     devices_changed_signal = QtCore.pyqtSignal(name="devicesChangedSignal")
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self._device_manager = DeviceManager()
         self._last_scan_error = None
         self._init_timers()
 
-    def _refresh_devices(self):
+    def _refresh_devices(self) -> None:
         prev = self._last_scan_error
         try:
             changed = self._device_manager.scan()
             self._last_scan_error = None
             if changed:
                 self.devices_changed_signal.emit()
         except DeviceManagerError as e:
             self._last_scan_error = e
 
         if str(prev) != str(self._last_scan_error):
             self.devices_changed_signal.emit()
             self.last_scan_error_changed_signal.emit()
 
-    def _init_timers(self):
+    def _init_timers(self) -> None:
         self._status_time = QTimer()
         self._status_time.timeout.connect(self._refresh_devices)
         self._status_time.start(2000)
         self._refresh_devices()
 
     @property
     def last_scan_error(self) -> DeviceManagerError | None:
```

### Comparing `labelle-1.2.1/src/labelle/lib/devices/usb_device.py` & `labelle-1.2.2/src/labelle/lib/devices/usb_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import logging
 import platform
-from typing import NoReturn
+from textwrap import dedent
+from typing import Any, NoReturn
 
 import usb
 
 from labelle.lib.constants import (
     DEV_VENDOR,
     HID_INTERFACE_CLASS,
     PRINTER_INTERFACE_CLASS,
@@ -31,67 +32,65 @@
     def __init__(self, dev: usb.core.Device) -> None:
         self._dev = dev
         self._intf = None
         self._devin = None
         self._devout = None
 
     @property
-    def hash(self):
-        try:
-            return (
-                f"<{self._dev.manufacturer}|{self._dev.product}"
-                f"|{self._dev.serial_number}>"
-            )
-        except (ValueError, usb.core.USBError):
-            return None
+    def hash(self) -> str:
+        return self.usb_id
 
-    def _get_dev_attribute(self, attr):
+    def _get_dev_attribute(self, attr: str) -> Any:
         try:
             return getattr(self._dev, attr)
         except (ValueError, usb.core.USBError):
             return None
 
     @property
-    def manufacturer(self):
+    def manufacturer(self) -> str | None:
         return self._get_dev_attribute("manufacturer")
 
     @property
-    def product(self):
+    def product(self) -> str | None:
         return self._get_dev_attribute("product")
 
     @property
-    def serial_number(self):
+    def serial_number(self) -> str | None:
         return self._get_dev_attribute("serial_number")
 
     @property
-    def id_vendor(self):
-        return self._get_dev_attribute("idVendor")
+    def id_vendor(self) -> int:
+        id_ = self._get_dev_attribute("idVendor")
+        if id_ is None:
+            raise UsbDeviceError("Could not get idVendor")
+        return id_
 
     @property
-    def id_product(self):
-        return self._get_dev_attribute("idProduct")
+    def id_product(self) -> int:
+        id_ = self._get_dev_attribute("idProduct")
+        if id_ is None:
+            raise UsbDeviceError("Could not get idProduct")
+        return id_
 
     @property
-    def vendor_product_id(self):
-        vendor_id = int(self.id_vendor)
-        product_id = int(self.id_product)
-        return f"{vendor_id:04x}:{product_id:04x}"
+    def vendor_product_id(self) -> str:
+        return f"{self.id_vendor:04x}:{self.id_product:04x}"
 
     @property
-    def usb_id(self):
+    def usb_id(self) -> str:
         bus = self._get_dev_attribute("bus")
         address = self._get_dev_attribute("address")
         return f"Bus {bus:03} Device {address:03}: ID {self.vendor_product_id}"
 
     @staticmethod
-    def _is_supported_vendor(dev: usb.core.Device):
+    def _is_supported_vendor(dev: usb.core.Device) -> bool:
         return dev.idVendor == DEV_VENDOR
 
     @property
-    def is_supported(self):
+    def is_supported(self) -> bool:
         return (
             self._is_supported_vendor(self._dev)
             and self.id_product in SUPPORTED_PRODUCTS
         )
 
     @staticmethod
     def supported_devices() -> set[UsbDevice]:
@@ -161,47 +160,49 @@
         # if Path("/etc/arch-release").exists():
         #     restart_udev_command = "sudo udevadm control --reload"
         # elif Path("/etc/lsb-release").exists():
         #     restart_udev_command = "sudo systemctl restart udev.service"
         # else:
         #     restart_udev_command = None
 
-        udev_rule = ", ".join(
+        udev_rule = ",'\\\n                     '".join(
             [
                 'ACTION=="add"',
                 'SUBSYSTEMS=="usb"',
-                f'ATTRS{{idVendor}}=="{self._dev.idVendor:04x}"',
-                f'ATTRS{{idProduct}}=="{self._dev.idProduct:04x}"',
+                f'ATTRS{{idVendor}}=="{self.id_vendor:04x}"',
+                f'ATTRS{{idProduct}}=="{self.id_product:04x}"',
                 'MODE="0666"',
             ]
         )
 
         msg = f"""
+
             You do not have sufficient access to the device. You probably want to add the a udev
             rule in /etc/udev/rules.d with the following command:
 
-            echo '{udev_rule}' | sudo tee /etc/udev/rules.d/91-labelle-{self._dev.idProduct:x}.rules
+                echo '{udev_rule}' \\
+                  | sudo tee /etc/udev/rules.d/91-labelle-{self.id_vendor:04x}-{self.id_product:04x}.rules
 
             Next, refresh udev with:
 
-            sudo udevadm control --reload-rules
-            sudo udevadm trigger --attr-match=idVendor="0922"
+                sudo udevadm control --reload-rules
+                sudo udevadm trigger --attr-match=idVendor="0922"
 
             Finally, turn your device off and back on again to activate the new permissions.
 
             If this still does not resolve the problem, you might need to reboot.
             In case rebooting is necessary, please report this at {GITHUB_ISSUE_UDEV}.
             We are still trying to figure out a simple procedure which works for everyone.
             In case you still cannot connect, or if you have any information or ideas, please
             post them at that link.
         """  # noqa: E501
-        LOG.error(msg)
-        raise UsbDeviceError("Insufficient access to the device")
+        msg = dedent(msg)
+        raise UsbDeviceError(msg)
 
-    def _set_configuration(self):
+    def _set_configuration(self) -> None:
         try:
             self._dev.get_active_configuration()
             LOG.debug("Active device configuration already found.")
         except usb.core.USBError:
             try:
                 self._dev.set_configuration()
                 LOG.debug("Device configuration set.")
@@ -209,15 +210,15 @@
                 if e.errno == 13:
                     raise UsbDeviceError("Access denied") from e
                 if e.errno == 16:
                     LOG.debug("Device is busy, but this is okay.")
                 else:
                     raise
 
-    def setup(self):
+    def setup(self) -> None:
         try:
             self._setup()
         except usb.core.USBError as e:
             raise UsbDeviceError(f"Failed setup USB device: {e}") from e
 
     def _setup(self):
         self._set_configuration()
@@ -268,27 +269,27 @@
             self._devin = None
             self._devout = None
             raise UsbDeviceError("The device endpoints not be found")
         self._intf = intf
         self._devin = devin
         self._devout = devout
 
-    def dispose(self):
+    def dispose(self) -> None:
         usb.util.dispose_resources(self._dev)
 
     def is_match(self, patterns: list[str] | None) -> bool:
         if patterns is None:
             return True
         match = True
         for pattern in patterns:
             pattern = pattern.lower()
             match &= (
-                pattern in self.manufacturer.lower()
-                or pattern in self.product.lower()
-                or pattern in self.serial_number.lower()
+                pattern in (self.manufacturer or "").lower()
+                or pattern in (self.product or "").lower()
+                or pattern in (self.serial_number or "").lower()
             )
         return match
 
     @property
     def devin(self):
         return self._devin
```

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/__init__.py` & `labelle-1.2.2/src/labelle/lib/render_engines/__init__.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/barcode_with_text.py` & `labelle-1.2.2/src/labelle/lib/render_engines/barcode_with_text.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/horizontally_combined.py` & `labelle-1.2.2/src/labelle/lib/render_engines/horizontally_combined.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/margins.py` & `labelle-1.2.2/src/labelle/lib/render_engines/margins.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/print_payload.py` & `labelle-1.2.2/src/labelle/lib/render_engines/print_payload.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/print_preview.py` & `labelle-1.2.2/src/labelle/lib/render_engines/print_preview.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/qr.py` & `labelle-1.2.2/src/labelle/lib/render_engines/qr.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     RenderEngine,
     RenderEngineException,
 )
 from labelle.lib.utils import draw_image, scaling
 
 
 class QrTooBigError(RenderEngineException):
-    def __init__(self):
+    def __init__(self) -> None:
         msg = "Too much information to store in the QR code"
         super().__init__(msg)
 
 
 class NoContentError(RenderEngineException):
     pass
```

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/render_engine.py` & `labelle-1.2.2/src/labelle/lib/render_engines/render_engine.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/test_pattern.py` & `labelle-1.2.2/src/labelle/lib/render_engines/test_pattern.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/lib/render_engines/text.py` & `labelle-1.2.2/src/labelle/lib/render_engines/text.py`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/resources/fonts/Carlito-Bold.ttf` & `labelle-1.2.2/src/labelle/resources/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/resources/fonts/Carlito-BoldItalic.ttf` & `labelle-1.2.2/src/labelle/resources/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/resources/fonts/Carlito-Italic.ttf` & `labelle-1.2.2/src/labelle/resources/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/resources/fonts/Carlito-Regular.ttf` & `labelle-1.2.2/src/labelle/resources/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/resources/fonts/LICENSE` & `labelle-1.2.2/src/labelle/resources/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/resources/icons/barcode_icon.png` & `labelle-1.2.2/src/labelle/resources/icons/barcode_icon.png`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/resources/icons/img_icon.png` & `labelle-1.2.2/src/labelle/resources/icons/img_icon.png`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/resources/icons/logo_small.png` & `labelle-1.2.2/src/labelle/resources/icons/logo_small.png`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/src/labelle/resources/icons/txt_icon.png` & `labelle-1.2.2/src/labelle/resources/icons/txt_icon.png`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/vendoring/patches/matplotlib.patch` & `labelle-1.2.2/vendoring/patches/matplotlib.patch`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/.gitignore` & `labelle-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/LICENSE` & `labelle-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/README.md` & `labelle-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `labelle-1.2.1/pyproject.toml` & `labelle-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     {name = "Tomer Shalev", email = "tshalev@proofpoint.com"},
     {name = "Ben Mares", email = "services-labelle@tensorial.com"},
     {name = "Tomek Szczęsny", email = "mctom@tlen.pl"},
 ]
 license = "Apache-2.0"
 license-file = "LICENSE"
 dependencies = [
-    "importlib-metadata; python_version<'3.8'",
     "platformdirs",
     "Pillow>=8.1.2,<11",
     "PyQRCode>=1.2.1,<2",
     "python-barcode>=0.13.1,<1",
     "pyusb",
     "PyQt6",
     "darkdetect",
@@ -79,16 +78,17 @@
 
 [testenv]
 commands =
   pip check
   pip freeze
   labelle --version
   labelle --help
+  python -c "import labelle.gui.gui; print('GUI import succeeded')"
   labelle --output console "single line"
-  labelle --output console_inverted "inverted"
+  labelle --output console-inverted "inverted"
   labelle --output console multiple lines
   labelle --output console --barcode "Barcode" --barcode-type code128
   labelle --output console --barcode-with-text "Barcode" --barcode-type code128 Caption
   labelle --output console --qr QR
   labelle --output console --qr QR Caption
   labelle --output console --picture ./labelle.png
```

### Comparing `labelle-1.2.1/PKG-INFO` & `labelle-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: labelle
-Version: 1.2.1
+Version: 1.2.2
 Summary: Open-source label printing software
 Project-URL: Homepage, https://github.com/labelle-org/labelle
 Project-URL: source, https://github.com/labelle-org/labelle
 Project-URL: tracker, https://github.com/labelle-org/labelle/issues
 Author-email: "Sebastian J. Bronner" <waschtl@sbronner.com>
 Maintainer-email: Tomer Shalev <tshalev@proofpoint.com>, Ben Mares <services-labelle@tensorial.com>, Tomek Szczęsny <mctom@tlen.pl>
 License-Expression: Apache-2.0
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Printing
 Requires-Python: <4,>=3.8
 Requires-Dist: darkdetect
-Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: pillow<11,>=8.1.2
 Requires-Dist: platformdirs
 Requires-Dist: pyqrcode<2,>=1.2.1
 Requires-Dist: pyqt6
 Requires-Dist: python-barcode<1,>=0.13.1
 Requires-Dist: pyusb
 Requires-Dist: typer
```

