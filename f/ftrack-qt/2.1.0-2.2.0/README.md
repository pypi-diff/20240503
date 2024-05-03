# Comparing `tmp/ftrack_qt-2.1.0.tar.gz` & `tmp/ftrack_qt-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack_qt-2.1.0.tar", max compression
+gzip compressed data, was "ftrack_qt-2.2.0.tar", max compression
```

## Comparing `ftrack_qt-2.1.0.tar` & `ftrack_qt-2.2.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    10176 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0      168 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/README.md
--rw-r--r--   0        0        0     1249 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      895 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/__init__.py
--rw-r--r--   0        0        0       57 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/__init__.py
--rw-r--r--   0        0        0       74 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/decorators/__init__.py
--rw-r--r--   0        0        0      369 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/decorators/threading.py
--rw-r--r--   0        0        0      988 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/layout/__init__.py
--rw-r--r--   0        0        0     1018 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/theme/__init__.py
--rw-r--r--   0        0        0     1186 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/threading/__init__.py
--rw-r--r--   0        0        0     3802 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/utils/widget/__init__.py
--rw-r--r--   0        0        0       57 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/__init__.py
--rw-r--r--   0        0        0       77 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/accordion/__init__.py
--rw-r--r--   0        0        0     8688 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/accordion/accordion_widget.py
--rw-r--r--   0        0        0      267 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/__init__.py
--rw-r--r--   0        0        0     3616 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py
--rw-r--r--   0        0        0     3987 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py
--rw-r--r--   0        0        0     4105 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/new_asset_input_widget.py
--rw-r--r--   0        0        0      132 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/__init__.py
--rw-r--r--   0        0        0    30910 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/entity_browser.py
--rw-r--r--   0        0        0     1887 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/file_browser.py
--rw-r--r--   0        0        0      257 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/__init__.py
--rw-r--r--   0        0        0     1519 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/circular_button.py
--rw-r--r--   0        0        0     4058 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/options_button.py
--rw-r--r--   0        0        0     7456 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/progress_button.py
--rw-r--r--   0        0        0      168 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/delegate/__init__.py
--rw-r--r--   0        0        0     1612 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py
--rw-r--r--   0        0        0      346 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/__init__.py
--rw-r--r--   0        0        0      927 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/file_dialog.py
--rw-r--r--   0        0        0     4942 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/modal_dialog.py
--rw-r--r--   0        0        0     6357 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py
--rw-r--r--   0        0        0     3103 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/styled_dialog.py
--rw-r--r--   0        0        0     3411 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/tab_dialog.py
--rw-r--r--   0        0        0      167 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/__init__.py
--rw-r--r--   0        0        0     5412 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/accordion_header_widget.py
--rw-r--r--   0        0        0     2963 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/session_header_widget.py
--rw-r--r--   0        0        0      207 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/__init__.py
--rw-r--r--   0        0        0      647 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/arrow_icon.py
--rw-r--r--   0        0        0     2244 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/material_icon.py
--rw-r--r--   0        0        0     2807 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/status_icon.py
--rw-r--r--   0        0        0       58 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/info/__init__.py
--rw-r--r--   0        0        0     2598 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/info/entity_info.py
--rw-r--r--   0        0        0       59 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/lines/__init__.py
--rw-r--r--   0        0        0     1124 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/lines/line_widget.py
--rw-r--r--   0        0        0       57 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/lists/__init__.py
--rw-r--r--   0        0        0     5294 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/lists/asset_list.py
--rw-r--r--   0        0        0       59 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/logos/__init__.py
--rw-r--r--   0        0        0     1059 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/logos/ftrack_logo.py
--rw-r--r--   0        0        0      118 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/models/__init__.py
--rw-r--r--   0        0        0     3461 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/models/table_model.py
--rw-r--r--   0        0        0      264 2024-04-02 08:38:46.328145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/__init__.py
--rw-r--r--   0        0        0     3085 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py
--rw-r--r--   0        0        0     6504 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/overlay_widget.py
--rw-r--r--   0        0        0      964 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/shaded_widget.py
--rw-r--r--   0        0        0      128 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/progress/__init__.py
--rw-r--r--   0        0        0     9602 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/progress/progress_widget.py
--rw-r--r--   0        0        0       70 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/search/__init__.py
--rw-r--r--   0        0        0     3540 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/search/collapsable_search_box.py
--rw-r--r--   0        0        0      392 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/__init__.py
--rw-r--r--   0        0        0     8610 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/asset_selector.py
--rw-r--r--   0        0        0     7908 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/context_selector.py
--rw-r--r--   0        0        0     3450 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/list_selector.py
--rw-r--r--   0        0        0     1507 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/status_selector.py
--rw-r--r--   0        0        0     1450 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/version_selector.py
--rw-r--r--   0        0        0      486 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/__init__.py
--rw-r--r--   0        0        0      816 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/asset_version_thumbnail.py
--rw-r--r--   0        0        0     5530 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py
--rw-r--r--   0        0        0     1846 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py
--rw-r--r--   0        0        0      878 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py
--rw-r--r--   0        0        0     5599 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py
--rw-r--r--   0        0        0     1149 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py
--rw-r--r--   0        0        0      116 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/user/__init__.py
--rw-r--r--   0        0        0     2422 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/user/ftrack_user.py
--rw-r--r--   0        0        0      115 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/views/__init__.py
--rw-r--r--   0        0        0     1567 2024-04-02 08:38:46.332145 ftrack_qt-2.1.0/source/ftrack_qt/widgets/views/table_view.py
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 ftrack_qt-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      168 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/README.md
+-rw-r--r--   0        0        0     1136 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/__init__.py
+-rw-r--r--   0        0        0       74 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/decorators/__init__.py
+-rw-r--r--   0        0        0      369 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/decorators/threading.py
+-rw-r--r--   0        0        0      988 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/layout/__init__.py
+-rw-r--r--   0        0        0     1149 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/theme/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/threading/__init__.py
+-rw-r--r--   0        0        0     4519 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/widget/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/accordion/__init__.py
+-rw-r--r--   0        0        0     9497 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/accordion/accordion_widget.py
+-rw-r--r--   0        0        0      267 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/__init__.py
+-rw-r--r--   0        0        0     3723 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py
+-rw-r--r--   0        0        0     4100 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py
+-rw-r--r--   0        0        0     4230 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/new_asset_input_widget.py
+-rw-r--r--   0        0        0      132 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/__init__.py
+-rw-r--r--   0        0        0    30840 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/entity_browser.py
+-rw-r--r--   0        0        0     2040 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/file_browser.py
+-rw-r--r--   0        0        0      257 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/__init__.py
+-rw-r--r--   0        0        0     1595 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/circular_button.py
+-rw-r--r--   0        0        0     4099 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/options_button.py
+-rw-r--r--   0        0        0     7300 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/progress_button.py
+-rw-r--r--   0        0        0      168 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/delegate/__init__.py
+-rw-r--r--   0        0        0     1716 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py
+-rw-r--r--   0        0        0      346 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/__init__.py
+-rw-r--r--   0        0        0     1003 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/file_dialog.py
+-rw-r--r--   0        0        0     4997 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/modal_dialog.py
+-rw-r--r--   0        0        0     6485 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py
+-rw-r--r--   0        0        0     3199 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/styled_dialog.py
+-rw-r--r--   0        0        0     3525 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/tab_dialog.py
+-rw-r--r--   0        0        0      167 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/__init__.py
+-rw-r--r--   0        0        0     6079 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/accordion_header_widget.py
+-rw-r--r--   0        0        0     3013 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/session_header_widget.py
+-rw-r--r--   0        0        0      207 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/__init__.py
+-rw-r--r--   0        0        0      723 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/arrow_icon.py
+-rw-r--r--   0        0        0     2461 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/material_icon.py
+-rw-r--r--   0        0        0     2869 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/status_icon.py
+-rw-r--r--   0        0        0       58 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/info/__init__.py
+-rw-r--r--   0        0        0     2687 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/info/entity_info.py
+-rw-r--r--   0        0        0       59 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/lines/__init__.py
+-rw-r--r--   0        0        0     1255 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/lines/line_widget.py
+-rw-r--r--   0        0        0       57 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/lists/__init__.py
+-rw-r--r--   0        0        0     5474 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/lists/asset_list.py
+-rw-r--r--   0        0        0       59 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/logos/__init__.py
+-rw-r--r--   0        0        0     1191 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/logos/ftrack_logo.py
+-rw-r--r--   0        0        0      118 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/models/__init__.py
+-rw-r--r--   0        0        0     3766 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/models/table_model.py
+-rw-r--r--   0        0        0      264 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/__init__.py
+-rw-r--r--   0        0        0     3221 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py
+-rw-r--r--   0        0        0     1684 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/overlay_widget.py
+-rw-r--r--   0        0        0     1074 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/shaded_widget.py
+-rw-r--r--   0        0        0      128 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/progress/__init__.py
+-rw-r--r--   0        0        0    12979 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/progress/progress_widget.py
+-rw-r--r--   0        0        0       70 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/search/__init__.py
+-rw-r--r--   0        0        0     3684 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/search/collapsable_search_box.py
+-rw-r--r--   0        0        0      392 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/__init__.py
+-rw-r--r--   0        0        0     8949 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/asset_selector.py
+-rw-r--r--   0        0        0     8032 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/context_selector.py
+-rw-r--r--   0        0        0     3526 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/list_selector.py
+-rw-r--r--   0        0        0     1712 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/status_selector.py
+-rw-r--r--   0        0        0     1571 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/version_selector.py
+-rw-r--r--   0        0        0      486 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/__init__.py
+-rw-r--r--   0        0        0      920 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/asset_version_thumbnail.py
+-rw-r--r--   0        0        0     5714 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py
+-rw-r--r--   0        0        0     1950 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py
+-rw-r--r--   0        0        0     1007 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py
+-rw-r--r--   0        0        0     5783 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py
+-rw-r--r--   0        0        0     1149 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py
+-rw-r--r--   0        0        0      116 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/user/__init__.py
+-rw-r--r--   0        0        0     2453 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/user/ftrack_user.py
+-rw-r--r--   0        0        0      115 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/views/__init__.py
+-rw-r--r--   0        0        0     1676 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/views/table_view.py
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 ftrack_qt-2.2.0/PKG-INFO
```

### Comparing `ftrack_qt-2.1.0/LICENSE.txt` & `ftrack_qt-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.1.0/pyproject.toml` & `ftrack_qt-2.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-qt"
-version = "2.1.0"
+version = "2.2.0"
 description='ftrack qt library'
 authors = ["ftrack Integrations Team <integrations@backlight.co>"]
 readme = "README.md"
 packages = [{include = "ftrack_qt", from = "source"}]
 license = "Apache-2.0"
 homepage = "https://ftrack.com"
 repository = "https://github.com/ftrackhq/integrations/tree/main/libs/qt"
@@ -20,23 +20,22 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = ">= 3.7, < 3.12"
-# TODO: PySide will be implemented in future versions
-PySide2 = { version = "^5.13.2", optional = true } #python = "<3.10", optional = true }
-#PySide6 = { version = "^6.5",  python = ">=3.10", optional = true }
-"Qt.py" = ">=1.0.0, < 2"
+PySide2 = { version = "^5.13.2", optional = true }
+PySide6 = { version = "^6.5", optional = true }
 #ftrack
-ftrack-constants= {  version = "^2.0.0", optional = true }
+ftrack-constants = {  version = "^2.0.0", optional = true }
 ftrack-utils = {  version = "^2.0.0", optional = true }
 ftrack-qt-style = {  version = "^2.0.0", optional = true }
 
 [tool.poetry.extras]
-pyside = ["PySide2"]
+pyside2 = ["PySide2"]
+pyside6 = ["PySide6"]
 ftrack-libs = ["ftrack-constants", "ftrack-utils", "ftrack-qt-style"]
 
 [tool.black]
 line-length = 79
 skip-string-normalization = true
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/__init__.py` & `ftrack_qt-2.2.0/source/ftrack_qt/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/utils/layout/__init__.py` & `ftrack_qt-2.2.0/source/ftrack_qt/utils/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/utils/theme/__init__.py` & `ftrack_qt-2.2.0/source/ftrack_qt/utils/theme/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 import sys
 
-from Qt import QtCore, QtWidgets, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui
 
 import ftrack_constants.qt as qt_constants
 
 
 def apply_font(font=':/ftrack/font/main'):
     '''Add application *font*.'''
     QtGui.QFontDatabase.addApplicationFont(font)
@@ -16,15 +19,17 @@
     '''Apply *theme* to *widget* - load stylesheet from resource file and apply'''
     apply_font()
     if theme is None:
         theme = qt_constants.theme.DEFAULT_THEME
     theme_path = ':/ftrack/style/{0}'.format(theme)
     fileObject = QtCore.QFile(theme_path)
     if fileObject.exists():
-        fileObject.open(QtCore.QFile.ReadOnly | QtCore.QFile.Text)
+        fileObject.open(
+            QtCore.QFile.OpenModeFlag.ReadOnly | QtCore.QFile.OpenModeFlag.Text
+        )
         stream = QtCore.QTextStream(fileObject)
         styleSheetContent = stream.readAll()
 
         widget.setStyleSheet(styleSheetContent)
     else:
         sys.stderr.write(
             'ftrack theme "{}" could not be found! Make sure to import '
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/utils/threading/__init__.py` & `ftrack_qt-2.2.0/source/ftrack_qt/utils/threading/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtCore, QtWidgets
+try:
+    from PySide6 import QtCore
+except ImportError:
+    from PySide2 import QtCore, QtWidgets
 
 
 class InvokeEvent(QtCore.QEvent):
     '''Event.'''
 
     def __init__(self, fn, *args, **kwargs):
         '''Invoke *fn* in main thread.'''
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/utils/widget/__init__.py` & `ftrack_qt-2.2.0/source/ftrack_qt/utils/widget/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-import shiboken2
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui
+    import shiboken6 as shiboken
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui
+    import shiboken2 as shiboken
 
 from ftrack_utils.framework.config.tool import get_plugins
 
 
 def check_framework_dialog_bases(cls):
     '''Recursively check the base classes for FrameworkDialog.'''
     for base in cls.__bases__:
@@ -35,22 +39,40 @@
 
     return main_dialog
 
 
 def set_property(widget, name, value):
     '''Update property *name* to *value* for *widget*, and polish afterwards.'''
     widget.setProperty(name, value)
-    if widget.style() is not None and shiboken2.isValid(
+    if widget.style() is not None and shiboken.isValid(
         widget.style()
     ):  # Only update style if applied and valid
         widget.style().unpolish(widget)
         widget.style().polish(widget)
     widget.update()
 
 
+def set_properties(widget, properties):
+    """
+    Set multiple properties on a Qt widget.
+
+    Args:
+        widget (QWidget): The widget on which to set the properties.
+        properties (dict): A dictionary of property names and values.
+    """
+    for name, value in properties.items():
+        widget.setProperty(name, value)
+        if widget.style() is not None and shiboken2.isValid(
+            widget.style()
+        ):  # Only update style if applied and valid
+            widget.style().unpolish(widget)
+            widget.style().polish(widget)
+        widget.update()
+
+
 def center_widget(widget, width=None, height=None):
     '''Returns a widget that is *widget* centered horizontally and vertically'''
     v_container = QtWidgets.QWidget()
     v_container.setLayout(QtWidgets.QVBoxLayout())
     v_container.layout().addWidget(QtWidgets.QLabel(""), 100)
 
     h_container = QtWidgets.QWidget()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/accordion/accordion_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/accordion/accordion_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.utils.widget import set_property
 from ftrack_qt.widgets.headers import AccordionHeaderWidget
 
 
 class AccordionBaseWidget(QtWidgets.QFrame):
     '''A utility accordion widget providing a header which can be expanded to show content'''
 
     clicked = QtCore.Signal(object)  # Emitted when accordion is clicked
     doubleClicked = QtCore.Signal(
         object
     )  # Emitted when accordion is double clicked
+    show_options_overlay = QtCore.Signal(object)
+    hide_options_overlay = QtCore.Signal()
 
     @property
     def title(self):
         '''Return the title text shown in header by default'''
         return self._title
 
     @property
@@ -123,15 +128,15 @@
         self._indicator_widget.setVisible(False)
 
         self.layout().addWidget(self._indicator_widget)
 
         # Create the main_widget
         main_widget = QtWidgets.QWidget()
         main_widget.setLayout(QtWidgets.QVBoxLayout())
-        main_widget.layout().setAlignment(QtCore.Qt.AlignTop)
+        main_widget.layout().setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
         main_widget.layout().setContentsMargins(0, 0, 0, 0)
         main_widget.layout().setSpacing(1)
 
         # Create Header
         self._header_widget = AccordionHeaderWidget(
             title=self.title,
             checkable=self.checkable,
@@ -160,17 +165,29 @@
         self._header_widget.checkbox_status_changed.connect(
             self._on_checkbox_status_changed
         )
         self._header_widget.clicked.connect(self._on_header_clicked)
         self._header_widget.arrow_clicked.connect(
             self._on_header_arrow_clicked
         )
+        self._header_widget.show_options_overlay.connect(
+            self._on_show_options_overlay_callback
+        )
+        self._header_widget.hide_options_overlay.connect(
+            self._on_hide_options_overlay_callback
+        )
         self._content_widget.setVisible(not self._collapsed)
         self._content_widget.setEnabled(self.checked)
 
+    def _on_show_options_overlay_callback(self, widget):
+        self.show_options_overlay.emit(widget)
+
+    def _on_hide_options_overlay_callback(self):
+        self.hide_options_overlay.emit()
+
     def add_option_widget(self, widget, section_name):
         self._header_widget.add_option_widget(widget, section_name)
 
     def add_widget(self, widget):
         '''Add widget to content'''
         self._content_widget.layout().addWidget(widget)
 
@@ -202,15 +219,15 @@
         '''Callback on enable checkbox user interaction'''
         self._checked = checked
         self._content_widget.setEnabled(self.checked)
 
     def _on_header_clicked(self, event):
         '''Callback on header user click'''
         if not self.selectable:
-            if event.button() != QtCore.Qt.RightButton:
+            if event.button() != (QtCore.Qt.MouseButton.RightButton):
                 self.toggle_collapsed()
 
     def _on_header_arrow_clicked(self, event):
         '''Callback on header arrow user click'''
         if self.selectable:
             # This is the way to collapse
             self.toggle_collapsed()
@@ -250,7 +267,12 @@
         '''Update accordion background depending on selection state'''
         if self.selectable:
             set_property(
                 self,
                 'background',
                 'selected' if self._selected else 'transparent',
             )
+
+    def teardown(self):
+        '''Teardown the header widget - properly cleanup the options overlay'''
+        self._header_widget.teardown()
+        self._header_widget.deleteLater()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.thumbnails import AssetVersionThumbnail
+from ftrack_qt.utils.widget import set_properties, set_property
 
 
 class AssetVersionCreation(QtWidgets.QFrame):
     '''Widget representing the next version of the asset version'''
 
     @property
     def version(self):
@@ -28,28 +32,34 @@
 
     @active.setter
     def active(self, value):
         '''Change active state of the widget - greys out the widget if False.'''
         if value == self._active:
             return
         self._active = value
-        self._asset_name_widget.style().unpolish(self._asset_name_widget)
-        self._create_label.style().unpolish(self._create_label)
-        self._version_label.style().unpolish(self._version_label)
         if value:
-            self._asset_name_widget.setObjectName('')
-            self._create_label.setObjectName('gray')
-            self._version_label.setObjectName('color-primary')
+            set_property(self._asset_name_widget, 'inactive', False)
+            set_properties(
+                self._create_label,
+                {'secondary': True, 'secondary_inactive': False},
+            )
+            set_properties(
+                self._version_label,
+                {'highlighted': True, 'secondary_inactive': False},
+            )
         else:
-            self._asset_name_widget.setObjectName('gray-dark')
-            self._create_label.setObjectName('gray-darker')
-            self._version_label.setObjectName('gray-darker')
-        self._asset_name_widget.style().polish(self._asset_name_widget)
-        self._create_label.style().polish(self._create_label)
-        self._version_label.style().polish(self._version_label)
+            set_property(self._asset_name_widget, 'inactive', True)
+            set_properties(
+                self._create_label,
+                {'secondary': False, 'secondary_inactive': True},
+            )
+            set_properties(
+                self._version_label,
+                {'highlighted': False, 'secondary_inactive': True},
+            )
 
     def __init__(self, asset_name, asset_id, versions, server_url):
         '''Initialize the AssetVersionCreation widget.'''
         super(AssetVersionCreation, self).__init__()
 
         self._asset_id = asset_id
         self._asset_name = asset_name
@@ -83,21 +93,21 @@
         )
         self.layout().addWidget(self._thumbnail_widget)
 
         self._asset_name_widget = QtWidgets.QLabel(self._asset_name)
         self.layout().addWidget(self._asset_name_widget)
 
         self._create_label = QtWidgets.QLabel('- create')
-        self._create_label.setObjectName('gray')
+        self._create_label.setProperty('secondary', True)
         self.layout().addWidget(self._create_label)
 
         self._version_label = QtWidgets.QLabel(
             'Version {}'.format(
                 self.version['next_version'] if self.version else "1"
             )
         )
-        self._version_label.setObjectName('color-primary')
-        self.layout().addWidget(self._version_label)
 
+        self._version_label.setProperty('highlighted', True)
+        self.layout().addWidget(self._version_label)
         self.layout().addStretch()
 
         self.setToolTip(self._asset_name)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
-from ftrack_qt.widgets.selectors.version_selector import VersionSelector
 from ftrack_qt.widgets.thumbnails import AssetVersionThumbnail
 
 
 class AssetVersionSelection(QtWidgets.QFrame):
     '''Widget representing an asset, with version selector, within the list,
     for user selection'''
 
@@ -57,14 +59,19 @@
         '''Set up the layout for the widget.'''
         self.setLayout(QtWidgets.QHBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().setSpacing(5)
 
     def build(self):
         '''Build the widget components.'''
+
+        from ftrack_qt.widgets.selectors.version_selector import (
+            VersionSelector,
+        )
+
         self._thumbnail_widget = AssetVersionThumbnail()
         self._thumbnail_widget.setScaledContents(True)
         self._thumbnail_widget.setMinimumSize(57, 31)
         self._thumbnail_widget.setMaximumSize(57, 31)
         self.layout().addWidget(self._thumbnail_widget)
 
         self._asset_name_widget = QtWidgets.QLabel(self._asset_name)
@@ -72,15 +79,15 @@
 
         self._version_combobox = VersionSelector()
         self._version_combobox.set_versions(self._versions)
         self._version_combobox.setMaximumHeight(20)
         self.layout().addWidget(self._version_combobox)
 
         self._version_info_widget = QtWidgets.QLabel()
-        self._version_info_widget.setObjectName('gray')
+        self._version_info_widget.setProperty('secondary', True)
         self.layout().addWidget(self._version_info_widget, 10)
 
         self._thumbnail_widget.set_server_url(self._server_url)
         self._thumbnail_widget.load(
             self._version_combobox.version['thumbnail']
         )
         self._version_info_widget.setText(
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/asset/new_asset_input_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/new_asset_input_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
+
 from ftrack_qt.utils.widget import set_property
 
 
 class NewAssetInput(QtWidgets.QFrame):
     '''Widget holding new asset input during publish'''
 
     active_changed = QtCore.Signal(object)
@@ -57,37 +61,39 @@
         self.layout().setContentsMargins(4, 1, 1, 1)
         self.layout().setSpacing(1)
         self.setMaximumHeight(32)
 
     def build(self):
         '''Build the button, name input, and version label.'''
         self._button = QtWidgets.QPushButton('NEW')
-        self._button.setStyleSheet('background: #FFDD86;')
+        self._button.setProperty('filled', True)
         self._button.setFixedSize(56, 30)
         self._button.setMaximumSize(56, 30)
 
         self.layout().addWidget(self._button)
 
         self._name = QtWidgets.QLineEdit()
+        self._name.setAttribute(QtCore.Qt.WA_MacShowFocusRect, False)
         self._name.setPlaceholderText(self._placeholder_name)
         self._name.setValidator(self._validator)
         self._name.setSizePolicy(
-            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Minimum
+            QtWidgets.QSizePolicy.Policy.Preferred,
+            QtWidgets.QSizePolicy.Policy.Minimum,
         )
         self._name.setVisible(False)
         self.layout().addWidget(self._name, 1000)
 
         self._version_label = QtWidgets.QLabel('- Version 1')
-        self._version_label.setObjectName('color-primary')
         self._version_label.setVisible(False)
         self.layout().addWidget(self._version_label)
 
         self._filler = QtWidgets.QLabel('')
         self._filler.setSizePolicy(
-            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
+            QtWidgets.QSizePolicy.Policy.Expanding,
+            QtWidgets.QSizePolicy.Policy.Minimum,
         )
         self.layout().addWidget(self._filler, 100)
 
     def post_build(self):
         '''Connect signals and callbacks after building.'''
         self._button.clicked.connect(self.input_clicked)
         self._name.mousePressEvent = self.input_clicked
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/entity_browser.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/entity_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 # :copyright: Copyright (c) 2024 ftrack
 
 # TODO: review this widget code and try to simplify it. Review all the utilities
 # as well in the same moment, I think we can simplify it a lot.
 
 from functools import partial
 
-from Qt import QtWidgets, QtCore, QtGui
-
-import shiboken2
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui
+    import shiboken6 as shiboken
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui
+    import shiboken2 as shiboken
 
 from ftrack_qt.widgets.thumbnails import ContextThumbnail
 from ftrack_qt.widgets.search import SearchBox
 from ftrack_qt.widgets.buttons import CircularButton
 from ftrack_qt.widgets.overlay import BusyIndicator
 from ftrack_qt.widgets.icons import MaterialIcon
 from ftrack_qt.widgets.dialogs import ModalDialog
@@ -401,18 +404,16 @@
 
     def _entity_selected(self, entity, double_click=False):
         '''User has selected an entity'''
         self._selected_entity = entity
         for entity_widget in self.entity_widgets:
             set_property(
                 entity_widget,
-                "background",
-                "selected"
-                if entity_widget.entity['id'] == entity['id']
-                else "",
+                "selected",
+                True if entity_widget.entity['id'] == entity['id'] else False,
             )
         if entity.entity_type != "Task":
             # Dive further down
             thread = BaseThread(
                 name='entity_clicked_thread',
                 target=self._on_set_intermediate_entity,
                 target_args=[entity],
@@ -663,24 +664,14 @@
         self.layout().addWidget(label)
         if self.link_entity['type'] != 'Project':
             self.layout().addStretch()
             self.remove_button = QtWidgets.QPushButton(
                 MaterialIcon('close', color='#94979a'), ""
             )
             self.remove_button.setFixedSize(8, 8)
-            self.remove_button.setStyleSheet(
-                '''
-            QPushButton {
-                border: none; background: transparent;
-            }
-            QPushButton:hover {
-                background: gray;
-            }
-'''
-            )
             self.layout().addWidget(self.remove_button)
 
     def post_build(self):
         fm = QtGui.QFontMetrics(self.font())
         self.setMinimumWidth(
             fm.horizontalAdvance(self.link_entity['name'])
             + (4 if self.link_entity['type'] != 'Project' else 0)
@@ -699,14 +690,16 @@
     clicked = QtCore.Signal()
     doubleClicked = QtCore.Signal()
 
     def __init__(
         self, entity, is_sub_task, entity_browser, parent=None, is_parent=False
     ):
         super(EntityWidget, self).__init__(parent=parent)
+        self.setProperty('selectable', True)
+        self.setProperty('border', True)
         self.entity = entity
         self.is_parent = is_parent
         self.is_sub_task = is_sub_task
         self._entity_browser = entity_browser
         self.pre_build()
         self.build()
         self.post_build()
@@ -731,28 +724,28 @@
         central_widget.layout().setContentsMargins(3, 0, 0, 0)
         central_widget.layout().setSpacing(0)
 
         # Context name
         label = QtWidgets.QLabel(
             self.entity['name'] if not self.is_parent else '..'
         )
-        label.setObjectName('h3' if not self.is_parent else 'h2')
+        label.setProperty('h3' if not self.is_parent else 'h2', True)
         central_widget.layout().addWidget(label)
 
         lower_widget = QtWidgets.QWidget()
         lower_widget.setLayout(QtWidgets.QHBoxLayout())
         lower_widget.layout().setContentsMargins(3, 0, 0, 0)
         lower_widget.layout().setSpacing(0)
 
         if self.is_sub_task and not self.is_parent:
             # Sub path
             sub_path = QtWidgets.QLabel(
                 '.. / {}'.format(self.entity['parent']['name'])
             )
-            sub_path.setObjectName('gray')
+            sub_path.setProperty('secondary', True)
             lower_widget.layout().addWidget(sub_path)
 
         if not self.is_parent:
             type_widget = TypeWidget(self.entity)
             lower_widget.layout().addWidget(type_widget)
 
         lower_widget.layout().addWidget(QtWidgets.QLabel(), 100)
@@ -781,29 +774,29 @@
                 }'''
                 % (self.entity['status']['color'])
             )
         self.setMinimumHeight(45 if not self.is_parent else 20)
         self.setMaximumHeight(45 if not self.is_parent else 20)
 
     def mousePressEvent(self, event):
-        if not shiboken2.isValid(self) or not shiboken2.isValid(
+        if not shiboken.isValid(self) or not shiboken.isValid(
             super(EntityWidget, self)
         ):
             # Widget has been destroyed
             return
         retval = super(EntityWidget, self).mousePressEvent(event)
         if (
             self._entity_browser is None
             or self._entity_browser.working is False
         ):
             self.clicked.emit()
         return retval
 
     def mouseDoubleClickEvent(self, event):
-        if not shiboken2.isValid(self) or not shiboken2.isValid(
+        if not shiboken.isValid(self) or not shiboken.isValid(
             super(EntityWidget, self)
         ):
             # Widget has been destroyed
             return
         return super(EntityWidget, self).mouseDoubleClickEvent(event)
         self.doubleClicked.emit()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/browsers/file_browser.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/file_browser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
 from pathlib import Path
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.dialogs import FileDialog
 
 
 class FileBrowser(QtWidgets.QWidget):
     '''Browse Widget is a line edit with a browse button'''
 
@@ -30,19 +33,20 @@
         self.setLayout(QtWidgets.QHBoxLayout())
         self.layout().setContentsMargins(15, 0, 0, 0)
         self.layout().setSpacing(0)
 
     def build(self):
         '''Build widgets'''
         self._path_le = QtWidgets.QLineEdit()
+        self._path_le.setAttribute(QtCore.Qt.WA_MacShowFocusRect, False)
 
         self.layout().addWidget(self._path_le, 20)
 
         self._browse_btn = QtWidgets.QPushButton('BROWSE')
-        self._browse_btn.setObjectName('borderless')
+        self._browse_btn.setProperty('borderless', True)
 
         self.layout().addWidget(self._browse_btn)
 
     def post_build(self):
         '''Connect widget signals'''
         self._browse_btn.clicked.connect(self._browse_button_clicked)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/circular_button.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/circular_button.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.icons import MaterialIcon
 
 
 class CircularButton(QtWidgets.QPushButton):
     '''Widget representing a circular button with an outline'''
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/options_button.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/options_button.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.overlay import OverlayWidget
 from ftrack_qt.widgets.lines import LineWidget
-from ftrack_qt.utils.widget import (
-    get_main_window_from_widget,
-    get_framework_main_dialog,
-)
 
 
 class OptionsButton(QtWidgets.QPushButton):
     '''Options button on publisher accordion'''
 
+    show_overlay_signal = QtCore.Signal(object)
+    hide_overlay_signal = QtCore.Signal()
+
     def __init__(self, title, icon, parent=None):
         '''
         Initialize options button
 
         :param title: The name of the step (component)
         :param icon: The button icon to use
         :param parent: the parent dialog or frame
@@ -43,69 +45,69 @@
 
     def build(self):
         self._main_widget = QtWidgets.QFrame()
         self._main_widget.setLayout(QtWidgets.QVBoxLayout())
         self._main_widget.layout().setAlignment(QtCore.Qt.AlignTop)
 
         title_label = QtWidgets.QLabel(self._title)
-        title_label.setObjectName('h2')
+        title_label.setProperty('h2', True)
         self._main_widget.layout().addWidget(title_label)
         self._main_widget.layout().addWidget(QtWidgets.QLabel(''))
+        self._main_widget.layout().setContentsMargins(0, 0, 0, 0)
 
         self._options_widget = QtWidgets.QWidget()
         self._options_widget.setLayout(QtWidgets.QVBoxLayout())
-        self._options_widget.layout().addWidget(
-            QtWidgets.QLabel(''), 100
-        )  # spacer
 
         scroll = QtWidgets.QScrollArea()
         scroll.setWidget(self._options_widget)
         scroll.setWidgetResizable(True)
         scroll.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
         scroll.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAsNeeded)
 
         self._main_widget.layout().addWidget(scroll)
-        self._overlay_container = OverlayWidget(
-            self._main_widget, height_percentage=0.9
+        # Add a vertical spacer at the end of the layout to push all widgets to the top
+        vertical_spacer = QtWidgets.QSpacerItem(
+            20,
+            40,
+            QtWidgets.QSizePolicy.Minimum,
+            QtWidgets.QSizePolicy.Expanding,
         )
-        self._overlay_container.setVisible(False)
+        self._main_widget.layout().addSpacerItem(vertical_spacer)
+
+        self._overlay_widget = OverlayWidget()
+
+        self._overlay_widget.set_widget(self._main_widget)
 
     def post_build(self):
         self.clicked.connect(self.on_click_callback)
+        self._overlay_widget.close_button_clicked.connect(
+            self._on_overlay_close_callback
+        )
 
     def on_click_callback(self):
         '''Callback on clicking the options button, show the publish options overlay'''
-        # Check first if widget is running on a ftrack framework dialog
-        main_window = get_framework_main_dialog(self)
-        if not main_window:
-            main_window = get_main_window_from_widget(self)
-        if main_window:
-            self._overlay_container.setParent(main_window)
-        self._overlay_container.setVisible(True)
+        self.show_overlay_signal.emit(self._overlay_widget)
+
+    def _on_overlay_close_callback(self):
+        '''Emits a hide_overlay_signal when overlay close button is clicked'''
+        self.hide_overlay_signal.emit()
 
     def add_widget(self, widget, section_name):
         if section_name not in self.__section_registry:
-            self._options_widget.layout().insertWidget(
-                self._options_widget.layout().count() - 1, LineWidget()
-            )
+            self._options_widget.layout().addWidget(LineWidget())
             section_label = QtWidgets.QLabel("{}:".format(section_name))
-            section_label.setObjectName('gray')
-            self._options_widget.layout().insertWidget(
-                self._options_widget.layout().count() - 1,
-                section_label,
-            )
+            section_label.setProperty('secondary', True)
+            self._options_widget.layout().addWidget(section_label)
             section_widget = QtWidgets.QWidget()
             section_widget_layout = QtWidgets.QVBoxLayout()
             section_widget.setLayout(section_widget_layout)
-            self._options_widget.layout().insertWidget(
-                self._options_widget.layout().count() - 1, section_widget
-            )
+            self._options_widget.layout().addWidget(section_widget)
 
-            # TODO: create the section Widget
             self.__section_registry[section_name] = section_widget
 
-        self.__section_registry[section_name].layout().insertWidget(
-            self._options_widget.layout().count() - 1, LineWidget()
-        )
-        self.__section_registry[section_name].layout().insertWidget(
-            self._options_widget.layout().count() - 1, widget
-        )
+        self.__section_registry[section_name].layout().addWidget(LineWidget())
+        self.__section_registry[section_name].layout().addWidget(widget)
+
+    def teardown(self):
+        '''Delete the overlay widget and main widget'''
+        self._main_widget.deleteLater()
+        self._overlay_widget.deleteLater()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/buttons/progress_button.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/progress_button.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 import ftrack_constants as constants
 from ftrack_qt.utils.widget import set_property
 from ftrack_qt.widgets.icons import StatusMaterialIconWidget
 from ftrack_qt.widgets.overlay import OverlayWidget
 
 
@@ -17,19 +20,18 @@
     def status(self):
         return self._status
 
     @status.setter
     def status(self, value):
         self._status = value
 
-    def __init__(self, style_mode, parent=None):
+    def __init__(self, parent=None):
         super(ProgressStatusButtonWidget, self).__init__(parent=parent)
 
         self._status = constants.status.UNKNOWN_STATUS
-        self._style_mode = style_mode
 
         self._message_label = None
         self._status_icon = None
 
         self.pre_build()
         self.build()
 
@@ -39,16 +41,14 @@
         layout.setSpacing(1)
         self.setLayout(layout)
 
         self.setMinimumHeight(32)
         self.setMinimumWidth(200)
 
     def build(self):
-        self.setObjectName(f'progress-widget-{self._style_mode}')
-
         self._message_label = QtWidgets.QLabel()
         self.layout().addWidget(self._message_label)
         self.layout().addStretch()
         self._status_icon = StatusMaterialIconWidget('')
         self.layout().addWidget(self._status_icon)
 
         self.set_status(constants.status.UNKNOWN_STATUS)
@@ -64,14 +64,17 @@
         color = self._status_icon.set_status(self.status, size=24)
         self._message_label.setStyleSheet(f'color: #{color}')
 
 
 class ProgressPhaseButtonWidget(QtWidgets.QPushButton):
     '''Showing progress of a progress phase, when pressed the log is shown.'''
 
+    show_overlay_signal = QtCore.Signal(object)
+    hide_overlay_signal = QtCore.Signal()
+
     @property
     def category(self):
         return self._category
 
     @property
     def label(self):
         return self._label
@@ -101,22 +104,20 @@
 
         self._label = label
         self._category = category
         self._tags = tags or []
         self._status = constants.status.UNKNOWN_STATUS
         self._log_message = None
 
-        self._log_overlay_container = None
         self._icon_widget = None
         self._status_message_widget = None
         self._log_message_widget = None
         self._log_text_edit = None
-        self._close_button = None
         self._time_widget = None
-        self.log_overlay_container = None
+        self._overlay_widget = None
 
         self.pre_build()
         self.build()
         self.post_build()
 
     def pre_build(self):
         layout = QtWidgets.QHBoxLayout()
@@ -131,67 +132,66 @@
         self._icon_widget = StatusMaterialIconWidget(None)
         self.layout().addWidget(self._icon_widget)
         self.set_status(self.status)
 
         v_layout = QtWidgets.QVBoxLayout()
 
         label_widget = QtWidgets.QLabel(self._label)
-        label_widget.setObjectName('h3')
+        label_widget.setProperty('h3', True)
         v_layout.addWidget(label_widget)
 
         # Show tags as chips
         h_layout = QtWidgets.QHBoxLayout()
         h_layout.setContentsMargins(0, 0, 0, 0)
 
         for tag in self._tags:
             tag_widget = QtWidgets.QLabel(tag)
-            tag_widget.setObjectName('gray')
+            tag_widget.setProperty('secondary', True)
             tag_widget.setStyleSheet(
                 'background: #333333; padding: 1px; border-radius: 6px;'
             )
             h_layout.addWidget(tag_widget)
         h_layout.addWidget(QtWidgets.QLabel(''), 100)  # Add spacing
 
         v_layout.addLayout(h_layout)
 
         self.layout().addLayout(v_layout, 100)
 
         v_layout = QtWidgets.QVBoxLayout()
 
         self._status_message_widget = QtWidgets.QLabel(self.status)
-        self._status_message_widget.setObjectName('gray')
+        self._status_message_widget.setProperty('secondary', True)
         v_layout.addWidget(self._status_message_widget)
 
         self._time_widget = QtWidgets.QLabel()
-        self._time_widget.setObjectName('gray')
+        self._time_widget.setProperty('secondary', True)
         v_layout.addWidget(self._time_widget)
 
         self.layout().addLayout(v_layout)
 
+        self._overlay_widget = OverlayWidget()
+
         self._log_message_widget = QtWidgets.QFrame()
         self._log_message_widget.setLayout(QtWidgets.QVBoxLayout())
         self._log_message_widget.layout().addSpacing(5)
         self._log_message_widget.layout().addWidget(
             QtWidgets.QLabel(f'{self.label} log:')
         )
 
         self._log_text_edit = QtWidgets.QTextEdit()
         self._log_text_edit.setReadOnly(True)
         self._log_message_widget.layout().addWidget(self._log_text_edit, 100)
-        self._close_button = QtWidgets.QPushButton('HIDE LOG')
-        self._log_message_widget.layout().addWidget(self._close_button)
-        self.log_overlay_container = OverlayWidget(
-            self._log_message_widget,
-            transparent_background=False,
-        )
-        self.log_overlay_container.setVisible(False)
+
+        self._overlay_widget.set_widget(self._log_message_widget)
 
     def post_build(self):
-        self.clicked.connect(self.show_log)
-        self._close_button.clicked.connect(self.hide_log)
+        self.clicked.connect(self._on_click_callback)
+        self._overlay_widget.close_button_clicked.connect(
+            self._on_overlay_close_callback
+        )
 
     def update_status(
         self, new_status, status_message, log_message, time=None
     ):
         '''Update the status of the phase to *new_status* and set *status_message*. 
         Build log messages from *log*.''' ''
         color = self.set_status(new_status)
@@ -205,23 +205,22 @@
 
     def set_status(self, new_status):
         '''Visualize *new_status* on the button'''
         self.status = new_status
         set_property(self, 'status', self.status.lower())
         return self._icon_widget.set_status(self.status)
 
+    def _on_click_callback(self):
+        '''Emits a show_overlay_signal when current widget is clicked'''
+        self.show_overlay_signal.emit(self._overlay_widget)
+        self.show_log()
+
+    def _on_overlay_close_callback(self):
+        '''Emits a hide_overlay_signal when overlay close button is clicked'''
+        self.hide_overlay_signal.emit()
+
     def show_log(self):
-        self.log_overlay_container.setParent(self.parent())
+        '''Sets the log message into the _log_text_edit'''
         if self.log_message:
             self._log_text_edit.setText(self.log_message)
         else:
             self._log_text_edit.setText("No errors found")
-        self.log_overlay_container.setVisible(True)
-        self.log_overlay_container.resize(self.parent().size())
-
-    def hide_log(self):
-        self.log_overlay_container.setVisible(False)
-
-    def teardown(self):
-        '''Teardown the progress button - close the overlay container'''
-        self.hide_log()
-        self.log_overlay_container.deleteLater()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 # TODO: try to generalize this delegate to be able to pass the looking keys.
 #  So it can be used in multiple places and not only for asset versions.
 
 
 class AssetVersionComboBoxDelegate(QtWidgets.QStyledItemDelegate):
     '''
@@ -27,15 +30,17 @@
         for asset_version in versions_collection:
             combo.addItem(str(asset_version['version']), asset_version)
 
         return combo
 
     def setEditorData(self, editor, index):
         '''Sets the given *data* into the given *editor*'''
-        editor_data = str(index.model().data(index, QtCore.Qt.EditRole))
+        editor_data = str(
+            index.model().data(index, QtCore.Qt.ItemDataRole.EditRole)
+        )
         idx = editor.findText(editor_data)
         editor.setCurrentIndex(idx)
 
     def setModelData(self, editor, model, index):
         '''
         Emits the signal index_changed when a new version is been selected
         '''
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/file_dialog.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/file_dialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 import os
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 
 class FileDialog(QtWidgets.QFileDialog):
     '''File dialog Widget'''
 
     caption = 'Choose file'
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/modal_dialog.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/modal_dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
 import platform
 
 from functools import partial
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 import ftrack_constants.qt as qt_constants
 
 from ftrack_qt.utils.widget import center_widget
 from ftrack_qt.widgets.dialogs import StyledDialog
 
 
@@ -47,27 +50,27 @@
 
         self.pre_build()
         self.build()
         self.post_build()
 
         self.setModal(True)
         self.setWindowFlags(
-            QtCore.Qt.SplashScreen | QtCore.Qt.WindowStaysOnTopHint
+            QtCore.Qt.WindowType.SplashScreen
+            | QtCore.Qt.WindowType.WindowStaysOnTopHint
         )
 
     def pre_build(self):
         self.setLayout(QtWidgets.QVBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().setSpacing(0)
 
     def build(self):
         '''Can be overridden by custom dialogs'''
         self._title_label = QtWidgets.QLabel()
         self._title_label.setAlignment(QtCore.Qt.AlignCenter)
-        self._title_label.setObjectName('titlebar')
         self.layout().addWidget(self._title_label)
         self._title_label.setMinimumHeight(24)
 
         self.layout().setSpacing(5)
 
         self.layout().addWidget(self.get_content_widget(), 100)
 
@@ -95,15 +98,15 @@
 
         self.layout().addWidget(buttonbar, 1)
 
     def get_content_widget(self):
         '''Create dialog main content widget, can be overridden to provide
         custom styled modal dialogs'''
         label = QtWidgets.QLabel(self._message)
-        label.setObjectName('h3')
+        label.setProperty('h3', True)
         return center_widget(label)
 
     def get_approve_button(self):
         '''Build the approve button widget, can be overridden to provide a
         custom approve button.'''
         button = QtWidgets.QPushButton(
             'YES' if self._question is True else 'OK'
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.selectors import ListSelector
 from ftrack_qt.widgets.headers import SessionHeader
 from ftrack_qt.widgets.selectors import ContextSelector
 
 from ftrack_qt.widgets.dialogs import StyledDialog
 
@@ -110,25 +113,27 @@
 
         self._tool_config_selector = ListSelector("Configs")
 
         self._scroll_area = QtWidgets.QScrollArea()
         self._scroll_area.setStyle(QtWidgets.QStyleFactory.create("plastique"))
         self._scroll_area.setWidgetResizable(True)
         self._scroll_area.setHorizontalScrollBarPolicy(
-            QtCore.Qt.ScrollBarAlwaysOff
+            QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff
         )
 
         self._tool_config_widget = QtWidgets.QWidget()
         _tool_config_widget_layout = QtWidgets.QVBoxLayout()
         self._tool_config_widget.setLayout(_tool_config_widget_layout)
 
         self._run_button = QtWidgets.QPushButton(self._run_button_title)
 
         self.layout().addWidget(self._header)
-        self.layout().addWidget(self._context_selector, QtCore.Qt.AlignTop)
+        self.layout().addWidget(
+            self._context_selector, QtCore.Qt.AlignmentFlag.AlignTop
+        )
         self.layout().addWidget(self._tool_config_selector)
         self.layout().addWidget(self._scroll_area, 100)
         self._scroll_area.setWidget(self._tool_config_widget)
         self.layout().addWidget(self._run_button)
 
     def post_build(self):
         '''Set up all the signals'''
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/styled_dialog.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/styled_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.overlay import ShadedWidget
 
 import ftrack_constants.qt as qt_constants
 from ftrack_qt.utils.theme import apply_theme
 
 
@@ -68,14 +71,14 @@
         # self.setWindowFlags(QtCore.Qt.Tool)
 
         self.setSizeGripEnabled(True)  # Enable resize on Windows
 
         apply_theme(self, self.theme)
         self.setProperty('background', self.background_style)
         self.setProperty('docked', 'true' if self.docked else 'false')
-        self.setAttribute(QtCore.Qt.WA_DeleteOnClose, True)
+        self.setAttribute(QtCore.Qt.WidgetAttribute.WA_DeleteOnClose, True)
 
         # Make sure the dialog is always on top
-        self.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
+        self.setWindowFlags(QtCore.Qt.WindowType.WindowStaysOnTopHint)
 
         # Have a proper title instead of default 'python'
         self.setWindowTitle('ftrack')
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/dialogs/tab_dialog.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/tab_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
+
 
 from ftrack_qt.widgets.selectors import ListSelector
 from ftrack_qt.widgets.headers import SessionHeader
 from ftrack_qt.widgets.selectors import ContextSelector
 
 from ftrack_qt.widgets.dialogs import StyledDialog
 
@@ -67,15 +71,18 @@
         self._context_selector = ContextSelector(
             self._session, enable_context_change=True
         )
 
         self._tab_widget = QtWidgets.QTabWidget()
 
         self.layout().addWidget(self._header)
-        self.layout().addWidget(self._context_selector, QtCore.Qt.AlignTop)
+
+        self.layout().addWidget(
+            self._context_selector, QtCore.Qt.AlignmentFlag.AlignTop
+        )
         self.layout().addWidget(self._tab_widget)
 
     def post_build(self):
         '''Set up all the signals'''
         # Connect context selector signals
         self._context_selector.context_changed.connect(
             self._on_context_selected_callback
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/accordion_header_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/accordion_header_widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.icons import (
     ArrowMaterialIconWidget,
     MaterialIcon,
     StatusMaterialIconWidget,
 )
 from ftrack_qt.widgets.lines import LineWidget
@@ -15,14 +18,16 @@
 class AccordionHeaderWidget(QtWidgets.QFrame):
     '''Container for accordion header - holding checkbox, title, user content
     and expander button.'''
 
     clicked = QtCore.Signal(object)  # User header click
     arrow_clicked = QtCore.Signal(object)  # User header click
     checkbox_status_changed = QtCore.Signal(object)
+    show_options_overlay = QtCore.Signal(object)
+    hide_options_overlay = QtCore.Signal()
 
     @property
     def title(self):
         return self._title
 
     @property
     def checkable(self):
@@ -40,14 +45,18 @@
     def collapsable(self):
         return self._collapsable
 
     @property
     def collapsed(self):
         return self._collapsed
 
+    @property
+    def options_button(self):
+        return self._options_button
+
     def __init__(
         self,
         title=None,
         checkable=False,
         checked=True,
         show_checkbox=False,
         collapsable=True,
@@ -92,40 +101,37 @@
         self._checkbox = QtWidgets.QCheckBox()
         self._checkbox.setEnabled(self.checkable)
         self._checkbox.setChecked(self.checked)
         self._checkbox.setVisible(self.show_checkbox)
 
         # Create title
         self._title_label = QtWidgets.QLabel(self.title or '')
-        self._title_label.setObjectName('borderless')
         if not self.title:
             self._title_label.hide()
 
         # Create Content
         self._header_content_widget = QtWidgets.QWidget()
         content_layout = QtWidgets.QHBoxLayout()
         content_layout.setContentsMargins(0, 0, 0, 0)
         content_layout.setSpacing(0)
         self._header_content_widget.setLayout(content_layout)
 
         # Add Status label widget in context Widget
         self._status_label = QtWidgets.QLabel()
-        self._status_label.setObjectName('color-primary')
         content_layout.addWidget(self._status_label)
         content_layout.addStretch()
         content_layout.addWidget(LineWidget(horizontal=True))
         # add options widget
         self._options_button = OptionsButton(
             self.title, MaterialIcon('settings', color='gray')
         )
-        self._options_button.setObjectName('borderless')
+        self._options_button.setProperty('borderless', True)
         content_layout.addWidget(LineWidget(horizontal=True))
         # add status icon
         self._status_icon = StatusMaterialIconWidget('check')
-        self._status_icon.setObjectName('borderless')
 
         # Create Arrow
         self._arrow = ArrowMaterialIconWidget(None)
         self.update_arrow_icon(self.collapsed)
         self._arrow.setVisible(self.collapsable)
 
         self.layout().addWidget(self._checkbox)
@@ -134,14 +140,26 @@
         self.layout().addWidget(self._options_button)
         self.layout().addWidget(self._status_icon)
         self.layout().addWidget(self._arrow)
 
     def post_build(self):
         self._checkbox.stateChanged.connect(self._on_checkbox_status_changed)
         self._arrow.clicked.connect(self._on_arrow_clicked)
+        self._options_button.show_overlay_signal.connect(
+            self.on_show_options_callback
+        )
+        self._options_button.hide_overlay_signal.connect(
+            self.on_hide_options_callback
+        )
+
+    def on_show_options_callback(self, widget):
+        self.show_options_overlay.emit(widget)
+
+    def on_hide_options_callback(self):
+        self.hide_options_overlay.emit()
 
     def add_option_widget(self, widget, section_name):
         self._options_button.add_widget(widget, section_name)
 
     def _on_checkbox_status_changed(self):
         self._checked = self._checkbox.isChecked()
         self._title_label.setEnabled(self._checked)
@@ -164,7 +182,12 @@
         '''(Override)'''
         self.clicked.emit(event)
         return super(AccordionHeaderWidget, self).mousePressEvent(event)
 
     def set_status(self, status, message):
         '''Set status message within header, to be implemented by child'''
         pass
+
+    def teardown(self):
+        '''Teardown the options button - properly cleanup the options overlay'''
+        self._options_button.teardown()
+        self._options_button.deleteLater()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/headers/session_header_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/session_header_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtCore, QtWidgets, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.logos import FtrackLogo as Logo
 from ftrack_qt.widgets.user import FtrackUser as User
 from ftrack_qt.utils.layout import recursive_clear_layout
 
 
 class SessionHeader(QtWidgets.QFrame):
@@ -30,38 +33,37 @@
         '''
         super(SessionHeader, self).__init__(parent=parent)
 
         self.session = session
         self._show_logo = show_logo
         self._title = title
         self._show_user = show_user
-        self.setObjectName('ftrack-header-widget')
 
         self.pre_build()
         self.build()
         self.post_build()
 
     def pre_build(self):
         self.setLayout(QtWidgets.QVBoxLayout())
         self.layout().setContentsMargins(8, 2, 7, 8)
-        self.layout().setAlignment(QtCore.Qt.AlignTop)
+        self.layout().setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
 
     def build(self):
         # Logo & User ID
         self.id_container = QtWidgets.QWidget(self)
         self.id_container_layout = QtWidgets.QHBoxLayout()
         self.id_container_layout.setContentsMargins(1, 1, 1, 1)
         self.id_container_layout.setSpacing(5)
-        self.id_container_layout.setAlignment(QtCore.Qt.AlignTop)
+        self.id_container_layout.setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
         self.id_container.setLayout(self.id_container_layout)
 
         self.logo = Logo(self)
         if len(self._title or ''):
             self._title_label = QtWidgets.QLabel(self._title)
-            self._title_label.setObjectName('h2')
+            self._title_label.setProperty('h2', True)
         self.content_container = QtWidgets.QWidget()
         self.content_container.setLayout(QtWidgets.QHBoxLayout())
         self.content_container.layout().setContentsMargins(0, 0, 0, 0)
         self.content_container.layout().setSpacing(0)
 
         self.user = User(self.session)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/arrow_icon.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/arrow_icon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.icons.status_icon import StatusMaterialIconWidget
 
 
 class ArrowMaterialIconWidget(StatusMaterialIconWidget):
     '''Custom material icon widget for arrow, emitting event on click'''
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/material_icon.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/material_icon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 import logging
 
-from Qt import QtCore, QtWidgets, QtGui, QtSvg
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui, QtSvg
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui, QtSvg
 
 
 class MaterialIcon(QtGui.QIcon):
     '''Material icon, displaying SVG material icon images'''
 
     def __init__(self, name, color=None, variant=None, parent=None):
         '''
@@ -26,28 +29,33 @@
         self.color = color
         if variant is None:
             variant = 'filled'
         resource_path = ':ftrack/image/material-design-icons/{}/{}'.format(
             variant, self._name
         )
         pixmap = None
-        if not color is None:
+        if color is not None:
             # Read SVG and add fill color
             inFile = QtCore.QFile(resource_path)
-            if inFile.open(QtCore.QFile.ReadOnly | QtCore.QFile.Text):
+            if inFile.open(
+                (
+                    QtCore.QFile.OpenModeFlag.ReadOnly
+                    | QtCore.QFile.OpenModeFlag.Text
+                )
+            ):
                 text_stream = QtCore.QTextStream(inFile)
                 svg_data = text_stream.readAll()
                 svg_data = svg_data.replace(
                     '/></svg>', ' fill="{}"/></svg>'.format(color)
                 )
                 svg_renderer = QtSvg.QSvgRenderer(
                     QtCore.QByteArray(bytearray(svg_data.encode()))
                 )
                 pixmap = QtGui.QPixmap(svg_renderer.defaultSize())
-                pixmap.fill(QtCore.Qt.transparent)
+                pixmap.fill(QtGui.Qt.GlobalColor.transparent)
                 painter = QtGui.QPainter(pixmap)
                 svg_renderer.render(painter)
                 painter.end()
             else:
                 self.logger.warning(
                     'Unknown material icon resource: {}!'.format(resource_path)
                 )
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/icons/status_icon.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/status_icon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 # TODO: clean this code
 import logging
 
-from Qt import QtCore, QtWidgets, QtGui, QtSvg
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 import ftrack_constants as constants
 from ftrack_qt.widgets.icons import MaterialIcon
 
 logger = logging.getLogger(__name__)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/info/entity_info.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/info/entity_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 import os
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 
 class EntityInfo(QtWidgets.QWidget):
     '''Widget presenting basic information about an entity(context)'''
 
     pathReady = QtCore.Signal(object)  # List if context parents are provided
 
@@ -54,23 +57,23 @@
     def build(self):
         name_widget = QtWidgets.QWidget()
         name_widget.setLayout(QtWidgets.QHBoxLayout())
         name_widget.layout().setContentsMargins(0, 0, 0, 0)
         name_widget.layout().setSpacing(0)
 
         self._name_field = QtWidgets.QLabel()
-        self._name_field.setObjectName('h3')
+        self._name_field.setProperty('h3', True)
         name_widget.layout().addWidget(self._name_field)
         if self._additional_widget:
             name_widget.layout().addWidget(self._additional_widget)
         name_widget.layout().addStretch()
         self.layout().addWidget(name_widget)
 
         self._path_field = QtWidgets.QLabel()
-        self._path_field.setObjectName('gray')
+        self._path_field.setProperty('secondary', True)
         self.layout().addWidget(self._path_field)
 
         self.layout().addStretch()
 
     def post_build(self):
         self.pathReady.connect(self._on_path_ready)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/lines/line_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/lines/line_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.utils.widget import set_property
 
 
 class LineWidget(QtWidgets.QFrame):
     '''Widget presenting a one pixel wide line'''
 
@@ -19,19 +22,21 @@
         '''
         super(LineWidget, self).__init__(parent=parent)
 
         if horizontal:
             self.setMaximumHeight(1)
             self.setMinimumHeight(1)
             self.setSizePolicy(
-                QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Minimum
+                QtWidgets.QSizePolicy.Policy.Preferred,
+                QtWidgets.QSizePolicy.Policy.Minimum,
             )
         else:
             self.setMaximumWidth(1)
             self.setMinimumWidth(1)
             self.setMaximumHeight(16)
             self.setMinimumHeight(16)
             self.setSizePolicy(
-                QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred
+                QtWidgets.QSizePolicy.Policy.Minimum,
+                QtWidgets.QSizePolicy.Policy.Preferred,
             )
         if style is not None:
             set_property(self, 'style', style)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/lists/asset_list.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/lists/asset_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
 import logging
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 
 class AssetList(QtWidgets.QListWidget):
     '''Widget presenting list of existing assets'''
 
     active_changed = QtCore.Signal(object)
     '''Signal emitted when the list is activated or deactivated, with active as argument.'''
@@ -60,18 +63,22 @@
         self.logger = logging.getLogger(
             __name__ + '.' + self.__class__.__name__
         )
         self.asset_list_widget_item_class = asset_list_widget_item_class
         self._latest_published_asset_item = None
         self._active = True
 
-        self.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
-        self.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
-        self.verticalScrollBar().setDisabled(True)
-        self.setAutoScroll(False)
+        self.setHorizontalScrollBarPolicy(
+            QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff
+        )
+        # TODO: Investigate further on how to make it look correctly
+        # self.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
+        # self.verticalScrollBar().setDisabled(True)
+        self.setAutoScroll(True)
+
         self.setSpacing(1)
         self.assets = []
         self.currentItemChanged.connect(self.on_item_changed_callback)
 
     def set_assets(self, assets):
         '''Set assets for the list'''
         self.currentItemChanged.disconnect()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/logos/ftrack_logo.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/logos/ftrack_logo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtCore, QtWidgets, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui
 
 
 class FtrackLogo(QtWidgets.QLabel):
     '''Header logo widget'''
 
     def __init__(self, parent=None):
         '''Instantiate logo widget.'''
@@ -14,23 +17,23 @@
         self.pre_build()
         self.build()
 
     def pre_build(self):
         self.setLayout(QtWidgets.QHBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().setSpacing(0)
-        self.layout().setAlignment(QtCore.Qt.AlignTop)
+        self.layout().setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
 
     def build(self):
         resource_path = ':ftrack/image/default/connectLogoDark'
         logoPixmap = QtGui.QPixmap(resource_path)
         if not logoPixmap is None:
             self.setPixmap(
                 logoPixmap.scaled(
                     QtCore.QSize(106, 32),
-                    QtCore.Qt.KeepAspectRatio,
-                    QtCore.Qt.SmoothTransformation,
+                    QtCore.Qt.AspectRatioMode.KeepAspectRatio,
+                    QtCore.Qt.TransformationMode.SmoothTransformation,
                 )
             )
             self.setPixmap(logoPixmap)
         else:
             self.setText("ftrack")
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/models/table_model.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/models/table_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 
 class TableModel(QtCore.QAbstractTableModel):
     '''Table model for generic data'''
 
-    DATA_ROLE = QtCore.Qt.UserRole + 1
+    DATA_ROLE = QtCore.Qt.ItemDataRole.UserRole + 1
 
     @property
     def data_items(self):
         '''
         Returns the :obj:`data_items`
         '''
         return self._data_items
@@ -56,60 +59,66 @@
 
         return len(self.data_items)
 
     def columnCount(self, parent):
         '''Return the column count for the internal data.'''
         return len(self._headers)
 
-    def data(self, index, role=QtCore.Qt.DisplayRole):
+    def data(self, index, role=QtCore.Qt.ItemDataRole.DisplayRole):
         '''Return the data provided in the given *index* and with *role*'''
 
         row = index.row()
         column = index.column()
 
         if not index.isValid():
             return None
 
         item = self.data_items[row]
         column_name = self._headers[column]
 
         # style versions
-        if role == QtCore.Qt.TextAlignmentRole and column == 0:
-            return QtCore.Qt.AlignCenter
+        if role == QtCore.Qt.ItemDataRole.TextAlignmentRole and column == 0:
+            return QtCore.Qt.AlignmentFlag.AlignCenter
 
         # style the rest
-        elif role == QtCore.Qt.DisplayRole:
+        elif role == QtCore.Qt.ItemDataRole.DisplayRole:
             if type(self._column_mapping[column_name]) == list:
                 # Small function to get the value from recursive keys
                 def get_recursive_keys(_item, keys):
                     if len(keys) == 1:
                         return _item[keys[0]]
                     return get_recursive_keys(_item[keys[0]], keys[1:])
 
                 return get_recursive_keys(
                     item, self._column_mapping[column_name]
                 )
             return str(item[self._column_mapping[column_name]])
 
-        elif role == QtCore.Qt.EditRole:
+        elif role == QtCore.Qt.ItemDataRole.EditRole:
             return item
 
         elif role == self.DATA_ROLE:
             return item
 
         return None
 
     def headerData(self, col, orientation, role):
         '''Provide header data'''
         if (
-            orientation == QtCore.Qt.Horizontal
-            and role == QtCore.Qt.DisplayRole
+            orientation == QtCore.Qt.Orientation.Horizontal
+            and role == QtCore.Qt.ItemDataRole.DisplayRole
         ):
             return self._headers[col].capitalize()
         return None
 
     def flags(self, index):
         '''Set :obj:`self._editable_columns` editable'''
         if index.column() in self._editable_columns:
-            return QtCore.Qt.ItemIsEditable | QtCore.Qt.ItemIsEnabled
+            return (
+                QtCore.Qt.ItemFlag.ItemIsEditable
+                | QtCore.Qt.ItemFlag.ItemIsEnabled
+            )
         else:
-            return QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsSelectable
+            return (
+                QtCore.Qt.ItemFlag.ItemIsEnabled
+                | QtCore.Qt.ItemFlag.ItemIsSelectable
+            )
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtSvg, QtGui
-import shiboken2
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui
+    import shiboken6 as shiboken
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui
+    import shiboken2 as shiboken
 
 
 class BusyIndicator(QtWidgets.QWidget):
     '''Widget implementing busy indicator - a spinning wheel'''
 
     def __init__(self, start=True, parent=None):
         '''Initialise indicator with optional *parent*.'''
@@ -26,15 +30,15 @@
         if self._timer is None:
             self._timer = self.startTimer(self._timerInterval)
         if not self.isVisible():
             self.setVisible(True)
 
     def stop(self):
         '''Stop spinning if currently spinning.'''
-        if shiboken2.isValid(self) and self._timer is not None:
+        if shiboken.isValid(self) and self._timer is not None:
             self.killTimer(self._timer)
             self._timer = None
 
     def timerEvent(self, event):
         '''Handle timer *event*.'''
         self._spinnerAngle += self._speed
         if self._spinnerAngle >= 360.0:
@@ -70,15 +74,15 @@
             )
 
             # Draw spinner at current spin angle.
             pen = QtGui.QPen()
             penWidth = 8.0
             pen.setWidth(penWidth)
             pen.setColor(self._spinnerColor)
-            pen.setCapStyle(QtCore.Qt.RoundCap)
+            pen.setCapStyle(QtCore.Qt.PenCapStyle.RoundCap)
 
             painter.setPen(pen)
 
             spinnerArea = QtCore.QRectF(
                 normalisedArea.top() + (penWidth / 2.0),
                 normalisedArea.left() + (penWidth / 2.0),
                 normalisedArea.width() - penWidth,
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/overlay/shaded_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/shaded_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui
 
 
 class ShadedWidget(QtWidgets.QWidget):
     '''The overlay widget used to shade the dialog'''
 
     def __init__(self, parent=None):
         super(ShadedWidget, self).__init__(parent=parent)
-        self.setWindowFlags(QtCore.Qt.FramelessWindowHint)
-        self.setAttribute(QtCore.Qt.WA_TranslucentBackground)
+        self.setWindowFlags(QtCore.Qt.WindowType.FramelessWindowHint)
+        self.setAttribute(QtCore.Qt.WidgetAttribute.WA_TranslucentBackground)
         self._fill_color = QtGui.QColor(19, 25, 32, 169)
 
     def paintEvent(self, event):
         super(ShadedWidget, self).paintEvent(event)
         # Get current window size and paint a semi transparent dark overlay across widget
         size = self.size()
         painter = QtGui.QPainter()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/progress/progress_widget.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/progress/progress_widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import logging
 
-from Qt import QtWidgets
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 import ftrack_constants as constants
 
 from ftrack_qt.utils.layout import recursive_clear_layout
 from ftrack_qt.widgets.overlay import OverlayWidget
 from ftrack_qt.widgets.buttons import (
     ProgressStatusButtonWidget,
@@ -21,15 +24,21 @@
     The widget is composed of a dialog header docked button widget and info button
     widget representing main status. Main area is a  scroll area containing detailed
     progress feedback in form of phases (plugin runs) grouped into categories
     (context, collector...).
 
     '''
 
-    MARGINS = 15
+    hide_overlay_signal = QtCore.Signal()
+    show_overlay_signal = QtCore.Signal()
+
+    @property
+    def overlay_widget(self):
+        '''Return the status widget'''
+        return self._overlay_widget
 
     @property
     def status_widget(self):
         '''Return the status widget'''
         return self._status_widget
 
     @property
@@ -45,71 +54,193 @@
     def __init__(self, action, data, parent=None):
         '''Initialise ProgressWidgetObject with *action* describing what progress
         represents and *data* containing information about the progress phases,
         with ptional *parent*'''
 
         super(ProgressWidget, self).__init__(parent=parent)
 
-        self._overlay_container = None
-        self._content_widget = None
-        self._status_banner = None
+        self._overlay_widget = None
+        self._progress_area = None
         self._status_widget = None
-        self._scroll = None
-        self._categories = []
-        self._phase_widgets = {}
-        self._main_window = None
+
         self._action = action
 
         self.logger = logging.getLogger(__name__)
 
         self.build()
         self.post_build()
 
         self.set_data(data)
 
     def build(self):
-        self._status_widget = ProgressStatusButtonWidget('header-button')
-        self._set_status_widget_visibility(False)
+        self._status_widget = ProgressStatusButtonWidget()
+        self._status_widget.setProperty('round', True)
+        self._status_widget.setVisible(False)
 
-        self._scroll = QtWidgets.QScrollArea()
-        self._scroll.setStyle(QtWidgets.QStyleFactory.create("plastique"))
-        self._scroll.setWidgetResizable(True)
+        self._overlay_widget = OverlayWidget()
 
-        self._content_widget = QtWidgets.QFrame()
-        self._content_widget.setObjectName('overlay')
-        self._content_widget.setLayout(QtWidgets.QVBoxLayout())
-        self._content_widget.layout().setContentsMargins(
-            self.MARGINS, self.MARGINS, self.MARGINS, self.MARGINS
+        self._progress_area = ProgressArea()
+        self._progress_area.set_action(self.action)
+
+        self._overlay_widget.set_widget(self._progress_area)
+
+    def post_build(self):
+        '''Wire up signals'''
+        self.status_widget.clicked.connect(self._on_status_widget_clicked)
+        self.overlay_widget.close_button_clicked.connect(
+            self._on_overlay_close
+        )
+        self._progress_area.status_updated.connect(self._on_status_updated)
+
+    def set_data(self, data):
+        '''Set the data for the progress widget, were *data* is a list of
+        dictionaries, one for each progress phase, with the following keys:
+            - id: Unique id of the phase
+            - label: A label for the phase
+            - category: (optional) The category of the phase
+            - tags: (optional) A list of tags for the phase
+            - indent: (optional) The indent level of the phase
+        '''
+        self._progress_area.set_data(data)
+
+    def _on_status_widget_clicked(self):
+        '''Emits a signal when status widget is clicked'''
+        self.show_overlay_signal.emit()
+
+    def _on_overlay_close(self):
+        '''Calls the hide overlay function when overlay close button is clicked'''
+        '''Hide the progress widget'''
+        self.hide_overlay()
+
+    def hide_overlay(self):
+        '''Hide the progress widget'''
+        self.hide_overlay_signal.emit()
+
+    # Run
+    def run(self):
+        '''Run progress widget on top of *main_widget*, with *action*'''
+        self._progress_area.reset_phase_statuses()
+        self.update_status(
+            constants.status.RUNNING_STATUS,
+            message=f'Running {self.action.lower()}...',
         )
 
-        self._scroll.setWidget(self._content_widget)
+    def update_status(self, new_status, message=None):
+        '''Set the new main status to *new_status*, with optional *message*'''
+        self.logger.debug(
+            f'Main status update: {new_status} (message: {message})'
+        )
+        self._progress_area.update_status(new_status, message)
+
+    def _on_status_updated(self, new_status, message):
+        '''Method call when status updated from progress area'''
+        self.status_widget.set_status(new_status, message=message)
+        self.status_widget.setVisible(True)
 
-        self._overlay_container = OverlayWidget(
-            self._scroll, height_percentage=0.8
+    def update_phase_status(
+        self,
+        id_,
+        new_status,
+        log_message='',
+        status_message=None,
+        time=None,
+    ):
+        '''Update the status of a phase/plugin *id_* to *new_status*, with
+        optional *log_message*, *status_message* and execution *time*'''
+        self._progress_area.update_phase_status(
+            id_, new_status, log_message, status_message, time
         )
-        self._overlay_container.setVisible(False)
 
-    def post_build(self):
-        '''Wire up signals'''
-        self.status_widget.clicked.connect(self.show_overlay)
+    def teardown(self):
+        '''Teardown the progress widget - properly cleanup the overlay containers'''
+        self._progress_area.teardown()
+
+
+class ProgressArea(QtWidgets.QScrollArea):
+    '''
+    Representation of all the execution phases on a scroll area
+    '''
+
+    status_updated = QtCore.Signal(object, object)
+
+    @property
+    def content_widget(self):
+        '''Return the status widget'''
+        return self._content_widget
+
+    @property
+    def action(self):
+        '''Return a descriptive name of the action that is being run'''
+        return self._action or ''
+
+    @property
+    def status(self):
+        '''Return a descriptive name of the action that is being run'''
+        return self._status or ''
+
+    def __init__(self, parent=None):
+        '''Initialise ProgressWidgetObject with *action* describing what progress
+        represents and *data* containing information about the progress phases,
+        with ptional *parent*'''
+
+        super(ProgressArea, self).__init__(parent=parent)
+
+        self._content_widget = None
+        self._content_widget_layout = None
+        self._stacked_widget = None
+        self._status_banner = None
+
+        self._categories = []
+        self._phase_widgets = {}
+
+        self._action = None
+        self._status = None
+
+        self.logger = logging.getLogger(__name__)
+
+        self.pre_build()
+        self.build()
+
+    def pre_build(self):
+        self.setStyle(QtWidgets.QStyleFactory.create("plastique"))
+        self.setWidgetResizable(True)
+
+    def build(self):
+        self._stacked_widget = QtWidgets.QStackedWidget()
+
+        self._content_widget = QtWidgets.QFrame()
+        self._content_widget_layout = QtWidgets.QVBoxLayout()
+        self._content_widget.setLayout(self._content_widget_layout)
+
+        self._content_widget.setLayout(self._content_widget_layout)
+
+        # Add widgets to the stacked widget
+        self._stacked_widget.addWidget(self._content_widget)
+
+        self.setWidget(self._stacked_widget)
+        self._stacked_widget.setCurrentIndex(0)
+
+    def set_action(self, action):
+        '''Sets action name'''
+        self._action = action
 
     def set_data(self, data):
         '''Set the data for the progress widget, were *data* is a list of
         dictionaries, one for each progress phase, with the following keys:
             - id: Unique id of the phase
             - label: A label for the phase
             - category: (optional) The category of the phase
             - tags: (optional) A list of tags for the phase
             - indent: (optional) The indent level of the phase
         '''
         assert data and isinstance(data, list), 'Data must be a list'
 
         recursive_clear_layout(self._content_widget.layout())
 
-        self._status_banner = ProgressStatusButtonWidget('overlay-banner')
+        self._status_banner = ProgressStatusButtonWidget()
         self._content_widget.layout().addWidget(self._status_banner)
 
         self._categories = []
         self._phase_widgets = {}
 
         for phase_data in data:
             assert phase_data.get(
@@ -124,73 +255,52 @@
             category = phase_data.get('category', '')
             tags = phase_data.get('tags')
             indent = phase_data.get('indent', 0)
 
             phase_button = ProgressPhaseButtonWidget(
                 label, category=category, tags=tags
             )
+            phase_button.hide_overlay_signal.connect(self.show_main_widget)
+            phase_button.show_overlay_signal.connect(self.show_overlay_widget)
             self._phase_widgets[id_] = phase_button
-            self._content_widget.layout().setContentsMargins(
-                self.MARGINS + indent * 10,
-                self.MARGINS,
-                self.MARGINS,
-                self.MARGINS,
-            )
             if category not in self._categories:
                 self._categories.append(category)
                 phase_category = QtWidgets.QLabel(category)
-                phase_category.setObjectName("gray")
                 self._content_widget.layout().addWidget(phase_category)
             self._content_widget.layout().addWidget(phase_button)
 
         self._content_widget.layout().addWidget(QtWidgets.QLabel(), 10)
 
-    def _set_status_widget_visibility(self, visibility=False):
-        '''Update the visibility of the progress widget'''
-        self.status_widget.setVisible(visibility)
-
-    def show_overlay(self, main_window=None):
-        '''Show the progress widget overlay on top of *main_window*'''
-        if main_window:
-            self._main_window = main_window
-            self._overlay_container.setParent(self._main_window)
-        self._overlay_container.setVisible(True)
-        self.status_widget.setVisible(True)
-
-    def hide_overlay(self):
-        '''Hide the progress widget'''
-        self.status_widget.setVisible(False)
+    def show_main_widget(self):
+        '''Show the main widget index 0 of stacked widget'''
+        self._stacked_widget.setCurrentIndex(0)
+
+    def show_overlay_widget(self, widget):
+        '''Sets the given *widget* as the index 1 of the stacked widget and
+        remove the previous one if it exists'''
+        if self._stacked_widget.widget(1):
+            self._stacked_widget.removeWidget(self._stacked_widget.widget(1))
+        self._stacked_widget.addWidget(widget)
+        self._stacked_widget.setCurrentIndex(1)
 
     # Run
-    def reset_statuses(self, new_status=None, status_message=''):
+
+    def reset_phase_statuses(self, new_status=None, status_message=''):
         '''Reset statuses of all progress phases'''
         if not new_status:
             new_status = constants.status.UNKNOWN_STATUS
         for phase_widget in list(self._phase_widgets.values()):
             phase_widget.update_status(new_status, status_message, None)
-            phase_widget.hide_log()
-
-    def run(self, main_widget):
-        '''Run progress widget on top of *main_widget*, with *action*'''
-        self.reset_statuses()
-        self.update_status(
-            constants.status.RUNNING_STATUS,
-            message=f'Running {self.action.lower()}...',
-        )
-        self.show_overlay(main_widget)
 
     def update_status(self, new_status, message=None):
         '''Set the new main status to *new_status*, with optional *message*'''
-        self.logger.debug(
-            f'Main status update: {new_status} (message: {message})'
-        )
-        self.status_widget.set_status(new_status, message=message)
         if self._status_banner:
             self._status_banner.set_status(new_status, message=message)
-        self._set_status_widget_visibility(True)
+        self._status = new_status
+        self.status_updated.emit(new_status, message)
 
     def update_phase_status(
         self,
         id_,
         new_status,
         log_message='',
         status_message=None,
@@ -251,12 +361,9 @@
                 self.update_status(
                     constants.status.SUCCESS_STATUS,
                     message=f'{self.action.title()} completed successfully',
                 )
 
     def teardown(self):
         '''Teardown the progress widget - properly cleanup the overlay containers'''
-        self.hide_overlay()
         for phase_widget in list(self._phase_widgets.values()):
-            phase_widget.teardown()
-        self._overlay_container.setVisible(False)
-        self._overlay_container.deleteLater()
+            phase_widget.deleteLater()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/search/collapsable_search_box.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/search/collapsable_search_box.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtGui, QtCore, QtWidgets
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.utils.widget import set_property
 from ftrack_qt.widgets.buttons import CircularButton
 from ftrack_qt.utils.layout import recursive_clear_layout
 
 
 class SearchBox(QtWidgets.QFrame):
@@ -69,22 +72,23 @@
         set_property(self, 'collapsed', 'true' if self._collapsed else 'false')
         if self._collapsed:
             # Just the circular search button
             self.layout().addStretch()
             self._input = None
             self._search_button = CircularButton('search')
         else:
-            self._search_button = CircularButton('search', diameter=30)
+            self._search_button = CircularButton('search', diameter=26)
 
         if self._collapsable:
             self.layout().addWidget(self._search_button)
 
         if not self._collapsed:
             # A bordered input field filling all space, with input and a clear button
             self._input = QtWidgets.QLineEdit()
+            self._input.setAttribute(QtCore.Qt.WA_MacShowFocusRect, False)
             self._input.setReadOnly(False)
             self._input.textChanged.connect(self._on_input_changed)
             self._input.setPlaceholderText("Type to search")
             self._input.setFocus()
             self.layout().addWidget(self._input, 100)
             if not self._collapsable:
                 self.layout().addWidget(self._search_button)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/asset_selector.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/asset_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
 import logging
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui
+    from PySide6.QtCore import QRegularExpression
+    from PySide6.QtGui import QRegularExpressionValidator
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui
+    from PySide2.QtGui import QRegExpValidator as QRegularExpressionValidator
+    from PySide2.QtCore import QRegExp as QRegularExpression
 
 from ftrack_qt.widgets.asset import (
     AssetVersionCreation,
     AssetVersionSelection,
     NewAssetInput,
 )
 from ftrack_qt.widgets.lists import AssetList
@@ -97,30 +104,30 @@
         super(OpenAssetSelector, self).__init__()
 
 
 class PublishAssetSelector(AssetSelectorBase):
     '''Asset selector tailored for publish, allows user to select and existing
     asset or input an asset name for creating a new asset.'''
 
-    VALID_ASSET_NAME = QtCore.QRegExp('[A-Za-z0-9_]+')
+    VALID_ASSET_NAME = QRegularExpression('[A-Za-z0-9_]+')
 
     new_asset = QtCore.Signal(object)
     '''This signal is emitted when a new asset is selected. It sends the
     new asset_name as argument.'''
 
     def __init__(
         self,
         parent=None,
     ):
         '''
         This method initialises the publish asset selector widget.
         '''
         self._list_and_input = None
         self._new_asset_input = None
-        self.validator = QtGui.QRegExpValidator(self.VALID_ASSET_NAME)
+        self.validator = QRegularExpressionValidator(self.VALID_ASSET_NAME)
         self.placeholder_name = "Asset Name..."
 
         super(PublishAssetSelector, self).__init__(parent=parent)
 
     def build(self):
         '''This method builds the asset list and new asset input and adds them
         to the layout.'''
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/context_selector.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/context_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 import logging
-import shiboken2
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+    import shiboken6 as shiboken
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
+    import shiboken2 as shiboken
 
 from ftrack_qt.widgets.info import EntityInfo
 
 from ftrack_qt.widgets.thumbnails import ContextThumbnail
 from ftrack_utils.threading import BaseThread
 from ftrack_qt.widgets.buttons import CircularButton
 
@@ -205,15 +209,15 @@
             'select link, name , parent, parent.name from Context where id '
             'is "{}"'.format(context_id)
         ).one()
         return context_entity
 
     def _on_entity_found_async(self, entity):
         '''(Run in background thread) Entity found callback'''
-        if not shiboken2.isValid(self):
+        if not shiboken.isValid(self):
             # Widget has been closed while entity fetched
             self._browsing_context = False
             return
         self.entity_found.emit(entity)
 
     def _on_entity_found(self, entity):
         '''Entity found callback, set entity'''
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/list_selector.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/list_selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
 import logging
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.buttons import CircularButton
 
 
 class ListSelector(QtWidgets.QWidget):
     current_item_changed = QtCore.Signal(object)
     refresh_clicked = QtCore.Signal()
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/status_selector.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/status_selector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtGui, QtCore, QtWidgets
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui
 
 
 class StatusSelector(QtWidgets.QComboBox):
     '''A custom QComboBox for selecting statuses.'''
 
     statuses_changed = QtCore.Signal(object)
 
@@ -31,17 +34,23 @@
     def set_statuses(self, statuses):
         '''Set the available statuses in the combo box.'''
         self.clear()
         for index, status in enumerate(statuses):
             self.addItem(status['name'].upper(), status)
             # TODO: color not working.
             color = QtGui.QColor(status['color'])
-            self.setItemData(index, color, QtCore.Qt.ForegroundRole)
             self.setItemData(
-                index, QtGui.QColor('#131920'), QtCore.Qt.BackgroundRole
+                index,
+                color,
+                QtCore.Qt.ItemDataRole.ForegroundRole,
+            )
+            self.setItemData(
+                index,
+                QtGui.QColor('#131920'),
+                QtCore.Qt.ItemDataRole.BackgroundRole,
             )
         self.setCurrentIndex(0)
 
     def set_status_by_name(self, name):
         '''Set the selected status by name.'''
         for index in range(self.count()):
             if self.itemData(index)['name'] == name:
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/selectors/version_selector.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/version_selector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 import logging
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore, QtGui
+except ImportError:
+    from PySide2 import QtWidgets, QtCore, QtGui
 
 
 class VersionSelector(QtWidgets.QComboBox):
     '''Version selector combobox'''
 
     @property
     def version(self):
@@ -40,9 +43,11 @@
             self._add_version(version)
         self.setCurrentIndex(0)
 
     def _add_version(self, version):
         '''Add a version to the combobox.'''
         self.addItem(str('v{}'.format(version['version'])), version)
         self.setItemData(
-            self.count() - 1, QtGui.QColor('#131920'), QtCore.Qt.BackgroundRole
+            self.count() - 1,
+            QtGui.QColor('#131920'),
+            QtCore.Qt.ItemDataRole.BackgroundRole,
         )
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
+# TODO: Clean this code
 import time
 import os
 import logging
 import urllib.request, urllib.parse, urllib.error
 
-from Qt import QtCore, QtGui, QtWidgets
-import shiboken2
+try:
+    from PySide6 import QtCore, QtWidgets, QtGui
+    import shiboken6 as shiboken
+except ImportError:
+    from PySide2 import QtCore, QtWidgets, QtGui
+    import shiboken2 as shiboken
 
 from ftrack_utils.threading import BaseThread
 
 # Cache of thumbnail images.
 IMAGE_CACHE = dict()
 
 
-class ThumbnailBase(QtWidgets.QLabel):
+class SessionThumbnailBase(QtWidgets.QLabel):
     '''Widget to load thumbnails from ftrack server.'''
 
     MAX_CONNECTIONS = 10  # Maximum number of parallel connections to allow
 
     thumbnailFetched = QtCore.Signal(object)
     thumbnailNotFound = QtCore.Signal()
 
     _connection_count = 0
 
-    def __init__(self, scale=True, parent=None):
-        super(ThumbnailBase, self).__init__(parent)
-        self._server_url = None
+    def __init__(self, session, scale=True, parent=None):
+        super(SessionThumbnailBase, self).__init__(parent)
+        self.session = session
         self._alive = True
         self._scale = scale
 
         self.logger = logging.getLogger(
             __name__ + '.' + self.__class__.__name__
         )
 
         # self._worker = None
         self.__loadingReference = None
         self.pre_build()
         self.post_build()
 
-    def set_server_url(self, server_url):
-        self._server_url = server_url
-        self.placholderThumbnail = self._server_url + '/img/thumbnail2.png'
-
     def pre_build(self):
         self.thumbnailCache = {}
-        self.setFrameStyle(QtWidgets.QFrame.StyledPanel)
-        self.setAlignment(QtCore.Qt.AlignCenter)
+        self.setFrameStyle(QtWidgets.QFrame.Shape.StyledPanel)
+        self.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+
+        self.placholderThumbnail = (
+            self.session.server_url + '/img/thumbnail2.png'
+        )
 
     def post_build(self):
         self.thumbnailFetched.connect(self._downloaded)
         self.thumbnailNotFound.connect(self.use_placeholder)
 
     def load(self, reference):
         '''Load thumbnail from *reference* and display it.'''
@@ -70,41 +75,44 @@
         )
         thread.start()
 
         self.__loadingReference = reference
 
     def _download_async(self, reference):
         '''(Run in background thread) Download image'''
-        while ThumbnailBase.MAX_CONNECTIONS <= ThumbnailBase._connection_count:
+        while (
+            SessionThumbnailBase.MAX_CONNECTIONS
+            <= SessionThumbnailBase._connection_count
+        ):
             time.sleep(0.01)
             # Thumbnail widget still active?
-            if not shiboken2.isValid(self):
+            if not shiboken.isValid(self):
                 return
-        ThumbnailBase._connection_count += 1
+        SessionThumbnailBase._connection_count += 1
         try:
             return self._download(reference)
         except urllib.error.URLError:
             # Not found
-            if not shiboken2.isValid(self):
+            if not shiboken.isValid(self):
                 # Thumbnail widget has been destroyed
                 return
             self.thumbnailNotFound.emit()
         finally:
-            ThumbnailBase._connection_count -= 1
+            SessionThumbnailBase._connection_count -= 1
 
     def _downloaded_async(self, html):
         '''(Run in background thread) Image has been downloaded, propagate to QT thread'''
-        if not shiboken2.isValid(self):
+        if not shiboken.isValid(self):
             # Thumbnail widget has been destroyed
             return
         self.thumbnailFetched.emit(html)
 
     def _downloaded(self, result):
         '''Handler worker finished event.'''
-        if not shiboken2.isValid(self):
+        if not shiboken.isValid(self):
             # Thumbnail widget has been destroyed
             return
         IMAGE_CACHE[self.__loadingReference] = result
         self._updatePixmapData(result)
 
         self.__loadingReference = None
 
@@ -125,15 +133,16 @@
         resource_path = ':ftrack/image/default/placeholderThumbnail'
         self._scaleAndSetPixmap(QtGui.QPixmap(resource_path))
 
     def _scaleAndSetPixmap(self, pixmap):
         '''Scale and set *pixmap*.'''
         if self._scale:
             scaled_pixmap = pixmap.scaledToWidth(
-                self.width(), mode=QtCore.Qt.SmoothTransformation
+                self.width(),
+                mode=QtCore.Qt.TransformationMode.SmoothTransformation,
             )
         else:
             scaled_pixmap = pixmap
         self.setPixmap(scaled_pixmap)
 
     def _safeDownload(self, url, opener_callback, timeout=5):
         '''Check *url* through the given *opener_callback*.
@@ -147,15 +156,15 @@
 
         return opener_callback(url, timeout=timeout)
 
     def _download(self, url):
         '''Return thumbnail file from *url*.'''
         if url:
             ftrackProxy = os.getenv('FTRACK_PROXY', '')
-            ftrackServer = self._server_url
+            ftrackServer = self.session._server_url
 
             if ftrackProxy != '':
                 if ftrackServer.startswith('https'):
                     httpHandle = 'https'
                 else:
                     httpHandle = 'http'
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 # TODO: Clean this code
 
 import urllib.request, urllib.parse, urllib.error
 
-from Qt import QtCore, QtGui, QtWidgets
+try:
+    from PySide6 import QtCore, QtWidgets
+except ImportError:
+    from PySide2 import QtCore, QtWidgets
 
 from ftrack_qt.widgets.thumbnails.session_base_thumbnail import (
     SessionThumbnailBase,
 )
 
 
 class ContextThumbnail(SessionThumbnailBase):
@@ -48,13 +51,13 @@
         return result_url
 
     def _scaleAndSetPixmap(self, pixmap):
         '''Scale and set *pixmap*.'''
         if self._scale:
             scaled_pixmap = pixmap.scaled(
                 self.size(),
-                QtCore.Qt.KeepAspectRatio,
-                QtCore.Qt.SmoothTransformation,
+                QtCore.Qt.AspectRatioMode.KeepAspectRatio,
+                QtCore.Qt.TransformationMode.SmoothTransformation,
             )
         else:
             scaled_pixmap = pixmap
         self.setPixmap(scaled_pixmap)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 # TODO: Clean this code
 
-from Qt import QtCore, QtGui, QtWidgets
+try:
+    from PySide6 import QtCore, QtWidgets, QtGui
+except ImportError:
+    from PySide2 import QtCore, QtWidgets, QtGui
 
 from ftrack_qt.widgets.thumbnails.session_base_thumbnail import (
     SessionThumbnailBase,
 )
 
 
 class EllipseThumbnailBase(SessionThumbnailBase):
     '''Thumbnail which is drawn as an ellipse.'''
 
     def paintEvent(self, event):
         '''Override paint event to make round thumbnails.'''
         painter = QtGui.QPainter(self)
-        painter.setRenderHints(QtGui.QPainter.Antialiasing, True)
+        painter.setRenderHints(
+            QtGui.QPainter.RenderHint.Antialiasing,
+            True,
+        )
 
         # TODO: when no image this raises an error because of the assigning of
         #  the empty pixmap. Find another way to solve this.
         brush = QtGui.QBrush(self.pixmap())
 
         painter.setBrush(brush)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
-# TODO: Clean this code
 import time
 import os
 import logging
 import urllib.request, urllib.parse, urllib.error
 
-from Qt import QtCore, QtGui, QtWidgets
-import shiboken2
+try:
+    from PySide6 import QtCore, QtWidgets, QtGui
+    import shiboken6 as shiboken
+except ImportError:
+    from PySide2 import QtCore, QtWidgets, QtGui
+    import shiboken2 as shiboken
 
 from ftrack_utils.threading import BaseThread
 
 # Cache of thumbnail images.
 IMAGE_CACHE = dict()
 
 
-class SessionThumbnailBase(QtWidgets.QLabel):
+class ThumbnailBase(QtWidgets.QLabel):
     '''Widget to load thumbnails from ftrack server.'''
 
     MAX_CONNECTIONS = 10  # Maximum number of parallel connections to allow
 
     thumbnailFetched = QtCore.Signal(object)
     thumbnailNotFound = QtCore.Signal()
 
     _connection_count = 0
 
-    def __init__(self, session, scale=True, parent=None):
-        super(SessionThumbnailBase, self).__init__(parent)
-        self.session = session
+    def __init__(self, scale=True, parent=None):
+        super(ThumbnailBase, self).__init__(parent)
+        self._server_url = None
         self._alive = True
         self._scale = scale
 
         self.logger = logging.getLogger(
             __name__ + '.' + self.__class__.__name__
         )
 
         # self._worker = None
         self.__loadingReference = None
         self.pre_build()
         self.post_build()
 
+    def set_server_url(self, server_url):
+        self._server_url = server_url
+        self.placholderThumbnail = self._server_url + '/img/thumbnail2.png'
+
     def pre_build(self):
         self.thumbnailCache = {}
-        self.setFrameStyle(QtWidgets.QFrame.StyledPanel)
-        self.setAlignment(QtCore.Qt.AlignCenter)
-
-        self.placholderThumbnail = (
-            self.session.server_url + '/img/thumbnail2.png'
-        )
+        self.setFrameStyle(QtWidgets.QFrame.Shape.StyledPanel)
+        self.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
 
     def post_build(self):
         self.thumbnailFetched.connect(self._downloaded)
         self.thumbnailNotFound.connect(self.use_placeholder)
 
     def load(self, reference):
         '''Load thumbnail from *reference* and display it.'''
@@ -71,44 +74,41 @@
         )
         thread.start()
 
         self.__loadingReference = reference
 
     def _download_async(self, reference):
         '''(Run in background thread) Download image'''
-        while (
-            SessionThumbnailBase.MAX_CONNECTIONS
-            <= SessionThumbnailBase._connection_count
-        ):
+        while ThumbnailBase.MAX_CONNECTIONS <= ThumbnailBase._connection_count:
             time.sleep(0.01)
             # Thumbnail widget still active?
-            if not shiboken2.isValid(self):
+            if not shiboken.isValid(self):
                 return
-        SessionThumbnailBase._connection_count += 1
+        ThumbnailBase._connection_count += 1
         try:
             return self._download(reference)
         except urllib.error.URLError:
             # Not found
-            if not shiboken2.isValid(self):
+            if not shiboken.isValid(self):
                 # Thumbnail widget has been destroyed
                 return
             self.thumbnailNotFound.emit()
         finally:
-            SessionThumbnailBase._connection_count -= 1
+            ThumbnailBase._connection_count -= 1
 
     def _downloaded_async(self, html):
         '''(Run in background thread) Image has been downloaded, propagate to QT thread'''
-        if not shiboken2.isValid(self):
+        if not shiboken.isValid(self):
             # Thumbnail widget has been destroyed
             return
         self.thumbnailFetched.emit(html)
 
     def _downloaded(self, result):
         '''Handler worker finished event.'''
-        if not shiboken2.isValid(self):
+        if not shiboken.isValid(self):
             # Thumbnail widget has been destroyed
             return
         IMAGE_CACHE[self.__loadingReference] = result
         self._updatePixmapData(result)
 
         self.__loadingReference = None
 
@@ -129,15 +129,16 @@
         resource_path = ':ftrack/image/default/placeholderThumbnail'
         self._scaleAndSetPixmap(QtGui.QPixmap(resource_path))
 
     def _scaleAndSetPixmap(self, pixmap):
         '''Scale and set *pixmap*.'''
         if self._scale:
             scaled_pixmap = pixmap.scaledToWidth(
-                self.width(), mode=QtCore.Qt.SmoothTransformation
+                self.width(),
+                mode=QtCore.Qt.TransformationMode.SmoothTransformation,
             )
         else:
             scaled_pixmap = pixmap
         self.setPixmap(scaled_pixmap)
 
     def _safeDownload(self, url, opener_callback, timeout=5):
         '''Check *url* through the given *opener_callback*.
@@ -151,15 +152,15 @@
 
         return opener_callback(url, timeout=timeout)
 
     def _download(self, url):
         '''Return thumbnail file from *url*.'''
         if url:
             ftrackProxy = os.getenv('FTRACK_PROXY', '')
-            ftrackServer = self.session._server_url
+            ftrackServer = self._server_url
 
             if ftrackProxy != '':
                 if ftrackServer.startswith('https'):
                     httpHandle = 'https'
                 else:
                     httpHandle = 'http'
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/user/ftrack_user.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/user/ftrack_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 # TODO: Clean this code
-from Qt import QtCore, QtWidgets, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.thumbnails import UserThumbnail as UserThumbnail
 
 # Cache of user names.
 NAME_CACHE = dict()
 
 
@@ -14,23 +17,21 @@
 
     def __init__(self, session, parent=None):
         '''Instantiate user name and logo widget using *username*.'''
 
         super(FtrackUser, self).__init__(parent=parent)
         self.session = session
 
-        self.setObjectName('ftrack-userid-widget')
-
         self.pre_build()
         self.build()
 
     def pre_build(self):
         self.setLayout(QtWidgets.QHBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
-        self.layout().setAlignment(QtCore.Qt.AlignRight)
+        self.layout().setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
 
     def build(self):
         username = self.session.api_user
         # self.label = QtWidgets.QLabel(self)
         self.image = UserThumbnail(self.session)
         self.image.setFixedSize(35, 35)
```

### Comparing `ftrack_qt-2.1.0/source/ftrack_qt/widgets/views/table_view.py` & `ftrack_qt-2.2.0/source/ftrack_qt/widgets/views/table_view.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_qt.widgets.models import TableModel
 
 
 class TableView(QtWidgets.QTableView):
     '''Generic table view to represent an item.'''
 
@@ -31,15 +34,17 @@
         self.post_build()
 
     def pre_build(self):
         '''Prepare general layout.'''
 
         self.verticalHeader().hide()
 
-        self.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
+        self.setSelectionBehavior(
+            QtWidgets.QAbstractItemView.SelectionBehavior.SelectRows
+        )
 
         self.horizontalHeader().setStretchLastSection(True)
 
     def build(self):
         '''Build widgets and parent them.'''
         self._generic_model = TableModel(
             column_mapping=self._column_mapping, parent=self
```

### Comparing `ftrack_qt-2.1.0/PKG-INFO` & `ftrack_qt-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: ftrack-qt
-Version: 2.1.0
+Version: 2.2.0
 Summary: ftrack qt library
 Home-page: https://ftrack.com
 License: Apache-2.0
 Author: ftrack Integrations Team
 Author-email: integrations@backlight.co
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ftrack-libs
-Provides-Extra: pyside
-Requires-Dist: PySide2 (>=5.13.2,<6.0.0) ; extra == "pyside"
-Requires-Dist: Qt.py (>=1.0.0,<2)
+Provides-Extra: pyside2
+Provides-Extra: pyside6
+Requires-Dist: PySide2 (>=5.13.2,<6.0.0) ; extra == "pyside2"
+Requires-Dist: PySide6 (>=6.5,<7.0) ; extra == "pyside6"
 Requires-Dist: ftrack-constants (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Requires-Dist: ftrack-qt-style (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Requires-Dist: ftrack-utils (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Project-URL: Repository, https://github.com/ftrackhq/integrations/tree/main/libs/qt
 Description-Content-Type: text/markdown
 
 # Qt
```

