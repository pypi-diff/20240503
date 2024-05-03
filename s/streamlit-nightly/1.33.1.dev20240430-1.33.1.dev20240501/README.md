# Comparing `tmp/streamlit_nightly-1.33.1.dev20240430.tar.gz` & `tmp/streamlit_nightly-1.33.1.dev20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.33.1.dev20240430.tar", last modified: Wed May  1 06:55:03 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.33.1.dev20240501.tar", last modified: Thu May  2 06:53:55 2024, max compression
```

## Comparing `streamlit_nightly-1.33.1.dev20240430.tar` & `streamlit_nightly-1.33.1.dev20240501.tar`

### file list

```diff
@@ -1,574 +1,574 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.128347 streamlit_nightly-1.33.1.dev20240430/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-01 06:55:03.128347 streamlit_nightly-1.33.1.dev20240430/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.016345 streamlit_nightly-1.33.1.dev20240430/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:55:03.128347 streamlit_nightly-1.33.1.dev20240430/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.020345 streamlit_nightly-1.33.1.dev20240430/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.020345 streamlit_nightly-1.33.1.dev20240430/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    11931 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.020345 streamlit_nightly-1.33.1.dev20240430/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.020345 streamlit_nightly-1.33.1.dev20240430/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.024345 streamlit_nightly-1.33.1.dev20240430/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.024345 streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.024345 streamlit_nightly-1.33.1.dev20240430/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33936 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.028345 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/altair_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14558 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    57049 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/arrow_altair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/arrow_vega_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    27801 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.032345 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51087 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    29664 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.036346 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31841 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17545 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17927 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26542 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22115 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    29836 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.036346 streamlit_nightly-1.33.1.dev20240430/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.036346 streamlit_nightly-1.33.1.dev20240430/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.036346 streamlit_nightly-1.33.1.dev20240430/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.036346 streamlit_nightly-1.33.1.dev20240430/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/material_icon_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.060346 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-01 06:51:23.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.064346 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.064346 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    17551 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.064346 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.064346 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29567 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.068346 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.068346 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.068346 streamlit_nightly-1.33.1.dev20240430/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-01 06:51:51.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.012345 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.068346 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/css/3092.95a45cfe.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/css/3466.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/css/43.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/css/main.3aaaea00.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.104347 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1168.fc5c673b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1307.8ea033f1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/178.7bea8c5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1792.b8efa879.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3636801 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2736.914069e5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32270 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3061.67758376.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    43574 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3092.bc07c48b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3466.05d62820.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3513.e3e7300a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3631.be5c35fa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4113.1e7eff4d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4253.749d5244.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/43.c6749504.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4319.bf1c86bf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4477.e10e4373.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4666.c4b22a63.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/474.87506447.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5345.65c91ee7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6013.64cd6d28.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2262785 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6150.427a30f5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   825783 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/656.7150a933.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/656.7150a933.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6853.3cbd385e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7217.d970c074.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7323.2808d029.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7602.e8abc06b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7805.51638fbc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8427.65ddaf36.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8477.7419a0aa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8492.3e609489.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8536.f13dff49.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9330.2b4c99e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9336.2d95d840.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9758.6e6d8662.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4402089 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/main.af77b7ba.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/main.af77b7ba.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.120347 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-01 06:55:00.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.120347 streamlit_nightly-1.33.1.dev20240430/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.120347 streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    47503 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.120347 streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.120347 streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.120347 streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.124347 streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.124347 streamlit_nightly-1.33.1.dev20240430/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.124347 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.124347 streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-01 06:55:01.000000 streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-05-01 06:55:01.000000 streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:55:01.000000 streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 06:55:01.000000 streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:51:20.000000 streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-01 06:55:01.000000 streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 06:55:01.000000 streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:55:03.124347 streamlit_nightly-1.33.1.dev20240430/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-01 06:49:52.000000 streamlit_nightly-1.33.1.dev20240430/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.662341 streamlit_nightly-1.33.1.dev20240501/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-02 06:53:55.662341 streamlit_nightly-1.33.1.dev20240501/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.550341 streamlit_nightly-1.33.1.dev20240501/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:53:55.662341 streamlit_nightly-1.33.1.dev20240501/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.554340 streamlit_nightly-1.33.1.dev20240501/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.554340 streamlit_nightly-1.33.1.dev20240501/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.554340 streamlit_nightly-1.33.1.dev20240501/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.558340 streamlit_nightly-1.33.1.dev20240501/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.558340 streamlit_nightly-1.33.1.dev20240501/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.558340 streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.558340 streamlit_nightly-1.33.1.dev20240501/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33936 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.566341 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/altair_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14558 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57049 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/arrow_altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/arrow_vega_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.566341 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.570341 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32277 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.570341 streamlit_nightly-1.33.1.dev20240501/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.570341 streamlit_nightly-1.33.1.dev20240501/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.570341 streamlit_nightly-1.33.1.dev20240501/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.570341 streamlit_nightly-1.33.1.dev20240501/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/material_icon_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.594341 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-02 06:50:11.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.598341 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.602341 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.602341 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.602341 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29567 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.602341 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.606341 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.606341 streamlit_nightly-1.33.1.dev20240501/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 06:50:39.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.546340 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.606341 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/css/3092.95a45cfe.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/css/3466.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/css/43.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/css/main.3aaaea00.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.638341 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1168.fc5c673b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1307.8ea033f1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/178.7bea8c5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1792.b8efa879.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3636801 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2736.914069e5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32270 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3061.67758376.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43574 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3092.bc07c48b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3466.05d62820.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3513.e3e7300a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3631.be5c35fa.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4113.1e7eff4d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4253.749d5244.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/43.c6749504.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4319.bf1c86bf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4477.e10e4373.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4666.c4b22a63.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/474.87506447.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5345.65c91ee7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6013.64cd6d28.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2262785 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6150.427a30f5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   825783 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/656.7150a933.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/656.7150a933.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6853.3cbd385e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7217.d970c074.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7323.2808d029.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7602.e8abc06b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7805.51638fbc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8427.65ddaf36.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8477.7419a0aa.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8492.3e609489.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8536.f13dff49.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9330.2b4c99e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9336.2d95d840.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9758.6e6d8662.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4402089 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/main.af77b7ba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/main.af77b7ba.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.654342 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-02 06:53:52.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.654342 streamlit_nightly-1.33.1.dev20240501/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.654342 streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47503 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.658342 streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.658342 streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.658342 streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.658342 streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.658342 streamlit_nightly-1.33.1.dev20240501/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.662341 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.662341 streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-02 06:53:54.000000 streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-05-02 06:53:54.000000 streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:53:54.000000 streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 06:53:54.000000 streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:50:08.000000 streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-02 06:53:54.000000 streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 06:53:54.000000 streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:53:55.662341 streamlit_nightly-1.33.1.dev20240501/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-02 06:48:36.000000 streamlit_nightly-1.33.1.dev20240501/tests/testutil.py
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/PKG-INFO` & `streamlit_nightly-1.33.1.dev20240501/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.33.1.dev20240430
+Version: 1.33.1.dev20240501
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/bin/streamlit.cmd` & `streamlit_nightly-1.33.1.dev20240501/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/setup.py` & `streamlit_nightly-1.33.1.dev20240501/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.33.1.dev20240430"  # PEP-440
+VERSION = "1.33.1.dev20240501"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/__main__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/case_converters.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/cli_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/code_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/color_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/column_config.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/commands/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/commands/execution_control.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/commands/page_config.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/commands/page_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -132,30 +132,58 @@
         be set once per page.
 
     Parameters
     ----------
     page_title: str or None
         The page title, shown in the browser tab. If None, defaults to the
         filename of the script ("app.py" would show "app • Streamlit").
-    page_icon : Anything supported by st.image or str or None
-        The page favicon.
-        Besides the types supported by `st.image` (like URLs or numpy arrays),
-        you can pass in an emoji as a string ("🦈") or a shortcode (":shark:").
-        If you're feeling lucky, try "random" for a random emoji!
-        Emoji icons are courtesy of Twemoji and loaded from MaxCDN.
+
+    page_icon : Anything supported by st.image, str, or None
+        The page favicon. If ``page_icon`` is ``None`` (default), the favicon
+        will be a monochrome Streamlit logo.
+
+        In addition to the types supported by ``st.image`` (like URLs or numpy
+        arrays), the following strings are valid:
+
+        * A single-character emoji. For example, you can set ``page_icon="🦈"``.
+
+        * An emoji short code. For example, you can set ``page_icon=":shark:"``.
+          For a list of all supported codes, see
+          https://share.streamlit.io/streamlit/emoji-shortcodes.
+
+        * The string literal, ``"random"``. You can set ``page_icon="random"``
+          to set a random emoji from the supported list above. Emoji icons are
+          courtesy of Twemoji and loaded from MaxCDN.
+
+        * An icon from the Material Symbols library (outlined style) in the
+          format ``":material/icon_name:"`` where "icon_name" is the name
+          of the icon in snake case.
+
+          For example, ``icon=":material/thumb_up:"`` will display the
+          Thumb Up icon. Find additional icons in the `Material Symbols \
+          <https://fonts.google.com/icons?icon.set=Material+Symbols&icon.style=Outlined>`_
+          font library.
+
+        .. note::
+            Colors are not supported for Material icons. When you use a
+            Material icon for favicon, it will be black, regardless of browser
+            theme.
+
     layout: "centered" or "wide"
         How the page content should be laid out. Defaults to "centered",
         which constrains the elements into a centered column of fixed width;
         "wide" uses the entire screen.
+
     initial_sidebar_state: "auto", "expanded", or "collapsed"
         How the sidebar should start out. Defaults to "auto",
         which hides the sidebar on small devices and shows it otherwise.
         "expanded" shows the sidebar initially; "collapsed" hides it.
         In most cases, you should just use "auto", otherwise the app will
         look bad when embedded and viewed on mobile.
+
     menu_items: dict
         Configure the menu that appears on the top-right side of this app.
         The keys in this dict denote the menu item you'd like to configure:
 
         - "Get help": str or None
             The URL this menu item should point to.
             If None, hides this menu item.
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/types/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/components.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/components/v1/custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/config.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/config_option.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/config_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/connections/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/connections/base_connection.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/connections/util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/constants.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/cursor.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/delta_generator.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/deprecation_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/development.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/echo.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/altair_utils.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/altair_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/arrow.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/arrow_altair.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/arrow_altair.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/arrow_vega_lite.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/arrow_vega_lite.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/balloons.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/code.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/dialog_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -90,64 +90,89 @@
     ...
 
 
 @gather_metrics("experimental_dialog")
 def dialog_decorator(
     title: F | None | str = "", *, width: DialogWidth = "small"
 ) -> F | Callable[[F], F]:
-    r"""Decorate a function to mark it as a Streamlit dialog. When the decorated function is called, a dialog element is inserted with the function's body as the content.
+    """Function decorator to create a modal dialog.
 
-    The decorated function can hold multiple elements which are rendered inside of a modal when the decorated function is called.
-    The decorated function is using `st.experimental_fragment`, which means that interacting with elements inside of the dialog will
-    only re-run the dialog function.
-
-    The decorated function can accept arguments that can be passed when it is called.
-
-    Dismissing a dialog does not cause an app re-run.
-    You can close the dialog programmatically by executing `st.rerun()` explicitly inside of the decorated function.
-
-    In order to pass state from dialog widgets to the app, you can leverage `st.session_state`.
+    A function decorated with ``@st.experimental_dialog`` becomes a dialog
+    function. When you call a dialog function, Streamlit inserts a modal dialog
+    into your app. Streamlit element commands called within the dialog function
+    render inside the modal dialog.
+
+    The dialog function can accept arguments that can be passed when it is
+    called. Any values from the dialog that need to be accessed from the wider
+    app should generally be stored in Session State.
+
+    A user can dismiss a modal dialog by clicking outside of it, clicking the
+    "**X**" in its upper-right corner, or pressing``ESC`` on their keyboard.
+    Dismissing a modal dialog does not trigger an app rerun. To close the modal
+    dialog programmatically, call ``st.rerun()`` explicitly inside of the
+    dialog function.
+
+    ``st.experimental_dialog`` inherits behavior from |st.experimental_fragment|_.
+    When a user interacts with an input widget created inside a dialog function,
+    Streamlit only reruns the dialog function instead of the full script.
+
+    Calling ``st.sidebar`` in a dialog function is not supported.
+
+    Dialog code can interact with Session State, imported modules, and other
+    Streamlit elements created outside the dialog. Note that these interactions
+    are additive across multiple dialog reruns. You are responsible for
+    handling any side effects of that behavior.
 
     .. warning::
-        Currently, a dialog may not open another dialog.
-        Also, only one dialog-decorated function may be called in a script run, which means that only one dialog can be open at any given time.
+        A dialog may not open another dialog. Only one dialog function may be
+        called in a script run, which means that only one dialog can be open at
+        any given time.
+
+    .. |st.experimental_fragment| replace:: ``st.experimental_fragment``
+    .. _st.experimental_fragment: https://docs.streamlit.io/develop/api-reference/execution-flow/st.fragment
 
     Parameters
     ----------
     title : str
-        A string that will be used as the dialog's title. It cannot be empty.
+        The title to display at the top of the modal dialog. It cannot be empty.
     width : "small", "large"
-        The width of the dialog. Defaults to "small".
-
-    Returns
-    -------
-    A decorated function that, when called, inserts a dialog element context container. The container itself contains the decorated function's elements.
+        The width of the modal dialog. If ``width`` is ``"small`` (default), the
+        modal dialog will be 500 pixels wide. If ``width`` is ``"large"``, the
+        modal dialog will be about 750 pixels wide.
 
     Examples
     --------
-    You can annotate a function to mark it as a Streamlit dialog function and pass arguments to it. You can either dismiss the dialog via the ESC-key or the X-button or close it programmatically and trigger a re-run by using `st.rerun()`.
-    Leverage `st.session_state` if you want to pass dialog widget states to the overall app:
+    The following example demonstrates the basic usage of ``@st.experimental_dialog``.
+    In this app, clicking "**A**" or "**B**" will open a modal dialog and prompt you
+    to enter a reason for your vote. In the modal dialog, click "**Submit**" to record
+    your vote into Session State and rerun the app. This will close the modal dialog
+    since the dialog function is not called during the full-script rerun.
 
     >>> import streamlit as st
     >>>
-    >>> @st.experimental_dialog("Streamlit Example Dialog")
-    >>> def example_dialog(some_arg: str, some_other_arg: int):
-    >>>     st.write(f"You passed following args: {some_arg} | {some_other_arg}")
-    >>>     # interacting with the text_input only re-runs `example_dialog`
-    >>>     some_text_input = st.text_input("Type something:", key="example_dialog_some_text_input")
-    >>>     # following write is updated when chaning the text_input inside the dialog
-    >>>     st.write(f"You wrote '{some_text_input}' in the dialog")
-    >>>     if st.button("Close the dialog"):
+    >>> @st.experimental_dialog("Cast your vote")
+    >>> def vote(item):
+    >>>     st.write(f"Why is {item} your favorite?")
+    >>>     reason = st.text_input("Because...")
+    >>>     if st.button("Submit"):
+    >>>         st.session_state.vote = {"item": item, "reason": reason}
     >>>         st.rerun()
     >>>
-    >>> if st.button("Open dialog"):
-    >>>     example_dialog("Some string arg", 42)
-    >>>
-    >>> # following write is updated with the dialog's text input when the dialog was opened, the text input was interacted with and a re-run was triggered, e.g. by clicking the Close-button defined in `example_dialog`
-    >>> st.write(f"You wrote '{st.session_state.get('example_dialog_some_text_input', '')}' in the dialog")
+    >>> if "vote" not in st.session_state:
+    >>>     st.write("Vote for your favorite")
+    >>>     if st.button("A"):
+    >>>         vote("A")
+    >>>     if st.button("B"):
+    >>>         vote("B")
+    >>> else:
+    >>>     f"You voted for {st.session_state.vote['item']} because {st.session_state.vote['reason']}"
+
+    .. output::
+        https://doc-dialog.streamlit.app/
+        height: 350px
 
     """
 
     func_or_title = title
     if func_or_title is None:
         # Support passing the params via function decorator
         def wrapper(f: F) -> F:
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/doc_string.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/empty.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/empty.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,20 +29,20 @@
         """Insert a single-element container.
 
         Inserts a container into your app that can be used to hold a single element.
         This allows you to, for example, remove elements at any point, or replace
         several elements at once (using a child multi-element container).
 
         To insert/replace/clear an element on the returned container, you can
-        use "with" notation or just call methods directly on the returned object.
+        use ``with`` notation or just call methods directly on the returned object.
         See examples below.
 
         Examples
         --------
-        Overwriting elements in-place using "with" notation:
+        Overwriting elements in-place using ``with`` notation:
 
         >>> import streamlit as st
         >>> import time
         >>>
         >>> with st.empty():
         ...     for seconds in range(60):
         ...         st.write(f"⏳ {seconds} seconds have passed")
@@ -78,15 +78,15 @@
         """Insert a single-element container which displays a "skeleton" placeholder.
 
         Inserts a container into your app that can be used to hold a single element.
         This allows you to, for example, remove elements at any point, or replace
         several elements at once (using a child multi-element container).
 
         To insert/replace/clear an element on the returned container, you can
-        use "with" notation or just call methods directly on the returned object.
+        use ``with`` notation or just call methods directly on the returned object.
         See some of the examples below.
 
         This is an internal method and should not be used directly.
 
         Parameters
         ----------
         height: int or None
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/exception.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/form.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         """Create a form that batches elements together with a "Submit" button.
 
         A form is a container that visually groups other elements and
         widgets together, and contains a Submit button. When the form's
         Submit button is pressed, all widget values inside the form will be
         sent to Streamlit in a batch.
 
-        To add elements to a form object, you can use "with" notation
+        To add elements to a form object, you can use ``with`` notation
         (preferred) or just call methods directly on the form. See
         examples below.
 
         Forms have a few constraints:
 
         * Every form must contain a ``st.form_submit_button``.
         * ``st.button`` and ``st.download_button`` cannot be added to a form.
@@ -153,15 +153,15 @@
                 Not showing a border can be confusing to viewers since interacting with a
                 widget in the form will do nothing. You should only remove the border if
                 there's another border (e.g. because of an expander) or the form is small
                 (e.g. just a text input and a submit button).
 
         Examples
         --------
-        Inserting elements using "with" notation:
+        Inserting elements using ``with`` notation:
 
         >>> import streamlit as st
         >>>
         >>> with st.form("my_form"):
         ...    st.write("Inside the form")
         ...    slider_val = st.slider("Form slider")
         ...    checkbox_val = st.checkbox("Form checkbox")
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/heading.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/heading.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,16 +65,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
         anchor : str or False
             The anchor name of the header that can be accessed with #anchor
             in the URL. If omitted, it generates an anchor using the body.
             If False, the anchor is not shown in the UI.
 
         help : str
@@ -136,16 +138,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
         anchor : str or False
             The anchor name of the header that can be accessed with #anchor
             in the URL. If omitted, it generates an anchor using the body.
             If False, the anchor is not shown in the UI.
 
         help : str
@@ -209,16 +213,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
         anchor : str or False
             The anchor name of the header that can be accessed with #anchor
             in the URL. If omitted, it generates an anchor using the body.
             If False, the anchor is not shown in the UI.
 
         help : str
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/html.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/iframe.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/image.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/json.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/layouts.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/layouts.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ) -> DeltaGenerator:
         """Insert a multi-element container.
 
         Inserts an invisible container into your app that can be used to hold
         multiple elements. This allows you to, for example, insert multiple
         elements into your app out of order.
 
-        To add elements to the returned container, you can use the "with" notation
+        To add elements to the returned container, you can use the ``with`` notation
         (preferred) or just call methods directly on the returned object. See
         examples below.
 
         Parameters
         ----------
         height : int or None
             Desired height of the container expressed in pixels. If ``None`` (default)
@@ -63,15 +63,15 @@
             Whether to show a border around the container. If ``None`` (default), a
             border is shown if the container is set to a fixed height and not
             shown otherwise.
 
 
         Examples
         --------
-        Inserting elements using "with" notation:
+        Inserting elements using ``with`` notation:
 
         >>> import streamlit as st
         >>>
         >>> with st.container():
         ...    st.write("This is inside the container")
         ...
         ...    # You can call any Streamlit command, including custom components:
@@ -147,15 +147,15 @@
         self, spec: SpecType, *, gap: str | None = "small"
     ) -> list[DeltaGenerator]:
         """Insert containers laid out as side-by-side columns.
 
         Inserts a number of multi-element containers laid out side-by-side and
         returns a list of container objects.
 
-        To add elements to the returned containers, you can use the "with" notation
+        To add elements to the returned containers, you can use the ``with`` notation
         (preferred) or just call methods directly on the returned object. See
         examples below.
 
         Columns can only be placed inside other columns up to one level of nesting.
 
         .. warning::
             Columns cannot be placed inside other columns in the sidebar. This is only possible in the main area of the app.
@@ -179,15 +179,15 @@
         Returns
         -------
         list of containers
             A list of container objects.
 
         Examples
         --------
-        You can use the `with` notation to insert any element into a column:
+        You can use the ``with`` notation to insert any element into a column:
 
         >>> import streamlit as st
         >>>
         >>> col1, col2, col3 = st.columns(3)
         >>>
         >>> with col1:
         ...    st.header("A cat")
@@ -273,15 +273,15 @@
     def tabs(self, tabs: Sequence[str]) -> Sequence[DeltaGenerator]:
         r"""Insert containers separated into tabs.
 
         Inserts a number of multi-element containers as tabs.
         Tabs are a navigational element that allows users to easily
         move between groups of related content.
 
-        To add elements to the returned containers, you can use the "with" notation
+        To add elements to the returned containers, you can use the ``with`` notation
         (preferred) or just call methods directly on the returned object. See
         examples below.
 
         .. warning::
             All the content of every tab is always sent to and rendered on the frontend.
             Conditional rendering is currently not supported.
 
@@ -301,29 +301,31 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
         Returns
         -------
         list of containers
             A list of container objects.
 
         Examples
         --------
-        You can use the `with` notation to insert any element into a tab:
+        You can use the ``with`` notation to insert any element into a tab:
 
         >>> import streamlit as st
         >>>
         >>> tab1, tab2, tab3 = st.tabs(["Cat", "Dog", "Owl"])
         >>>
         >>> with tab1:
         ...    st.header("A cat")
@@ -386,15 +388,15 @@
     def expander(self, label: str, expanded: bool = False) -> DeltaGenerator:
         r"""Insert a multi-element container that can be expanded/collapsed.
 
         Inserts a container into your app that can be used to hold multiple elements
         and can be expanded or collapsed by the user. When collapsed, all that is
         visible is the provided label.
 
-        To add elements to the returned container, you can use the "with" notation
+        To add elements to the returned container, you can use the ``with`` notation
         (preferred) or just call methods directly on the returned object. See
         examples below.
 
         .. warning::
             Currently, you may not put expanders inside another expander.
 
         Parameters
@@ -412,56 +414,58 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
         expanded : bool
             If True, initializes the expander in "expanded" state. Defaults to
             False (collapsed).
 
         Examples
         --------
-        You can use the `with` notation to insert any element into an expander
+        You can use the ``with`` notation to insert any element into an expander
 
         >>> import streamlit as st
         >>>
         >>> st.bar_chart({"data": [1, 5, 2, 6, 2, 1]})
         >>>
         >>> with st.expander("See explanation"):
-        ...     st.write(\"\"\"
+        ...     st.write('''
         ...         The chart above shows some numbers I picked for you.
         ...         I rolled actual dice for these, so they're *guaranteed* to
         ...         be random.
-        ...     \"\"\")
+        ...     ''')
         ...     st.image("https://static.streamlit.io/examples/dice.jpg")
 
         .. output ::
             https://doc-expander.streamlit.app/
             height: 750px
 
         Or you can just call methods directly on the returned objects:
 
         >>> import streamlit as st
         >>>
         >>> st.bar_chart({"data": [1, 5, 2, 6, 2, 1]})
         >>>
         >>> expander = st.expander("See explanation")
-        >>> expander.write(\"\"\"
+        >>> expander.write('''
         ...     The chart above shows some numbers I picked for you.
         ...     I rolled actual dice for these, so they're *guaranteed* to
         ...     be random.
-        ... \"\"\")
+        ... ''')
         >>> expander.image("https://static.streamlit.io/examples/dice.jpg")
 
         .. output ::
             https://doc-expander.streamlit.app/
             height: 750px
 
         """
@@ -519,16 +523,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
                 must be on their own lines). Supported LaTeX functions are listed
                 at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
         help : str
             An optional tooltip that gets displayed when the popover button is
@@ -541,15 +547,15 @@
         use_container_width : bool
             An optional boolean, which makes the popover button stretch its width
             to match the parent container. This only affects the button and not
             the width of the popover container.
 
         Examples
         --------
-        You can use the `with` notation to insert any element into a popover:
+        You can use the ``with`` notation to insert any element into a popover:
 
         >>> import streamlit as st
         >>>
         >>> with st.popover("Open popover"):
         >>>     st.markdown("Hello World 👋")
         >>>     name = st.text_input("What's your name?")
         >>>
@@ -605,19 +611,19 @@
         Inserts a container into your app that is typically used to show the status and
         details of a process or task. The container can hold multiple elements and can
         be expanded or collapsed by the user similar to ``st.expander``.
         When collapsed, all that is visible is the status icon and label.
 
         The label, state, and expanded state can all be updated by calling ``.update()``
         on the returned object. To add elements to the returned container, you can
-        use "with" notation (preferred) or just call methods directly on the returned
+        use ``with`` notation (preferred) or just call methods directly on the returned
         object.
 
         By default, ``st.status()`` initializes in the "running" state. When called using
-        "with" notation, it automatically updates to the "complete" state at the end
+        ``with`` notation, it automatically updates to the "complete" state at the end
         of the "with" block. See examples below for more details.
 
         Parameters
         ----------
 
         label : str
             The initial label of the status container. The label can optionally
@@ -632,16 +638,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents)
             render. Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
         expanded : bool
             If True, initializes the status container in "expanded" state. Defaults to
@@ -663,49 +671,49 @@
         StatusContainer
             A mutable status container that can hold multiple elements. The label, state,
             and expanded state can be updated after creation via ``.update()``.
 
         Examples
         --------
 
-        You can use the `with` notation to insert any element into an status container:
+        You can use the ``with`` notation to insert any element into an status container:
 
         >>> import time
         >>> import streamlit as st
         >>>
         >>> with st.status("Downloading data..."):
         ...     st.write("Searching for data...")
         ...     time.sleep(2)
         ...     st.write("Found URL.")
         ...     time.sleep(1)
         ...     st.write("Downloading data...")
         ...     time.sleep(1)
         >>>
-        >>> st.button('Rerun')
+        >>> st.button("Rerun")
 
         .. output ::
             https://doc-status.streamlit.app/
             height: 300px
 
-        You can also use `.update()` on the container to change the label, state,
+        You can also use ``.update()`` on the container to change the label, state,
         or expanded state:
 
         >>> import time
         >>> import streamlit as st
         >>>
         >>> with st.status("Downloading data...", expanded=True) as status:
         ...     st.write("Searching for data...")
         ...     time.sleep(2)
         ...     st.write("Found URL.")
         ...     time.sleep(1)
         ...     st.write("Downloading data...")
         ...     time.sleep(1)
         ...     status.update(label="Download complete!", state="complete", expanded=False)
         >>>
-        >>> st.button('Rerun')
+        >>> st.button("Rerun")
 
         .. output ::
             https://doc-status-update.streamlit.app/
             height: 300px
 
         """
         # We need to import StatusContainer here to avoid a circular import
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/column_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,17 @@
 
         * ``None`` (default) to display the URL itself.
 
         * A string that is displayed in every cell, e.g. ``"Open link"``.
 
         * A regular expression (JS flavor, detected by usage of parentheses)
           to extract a part of the URL via a capture group, e.g. ``"https://(.*?)\\.example\\.com"``
-          to extract the display text "foo" from the URL "https://foo.example.com".
+          to extract the display text "foo" from the URL "\\https://foo.example.com".
+
+        .. Comment: The backslash in front of foo.example.com prevents a hyperlink.
 
         For more complex cases, you may use `Pandas Styler's format \
         <https://pandas.pydata.org/docs/reference/api/pandas.io.formats.style.Styler.format.html>`_
         function on the underlying dataframe. Note that this makes the app slow,
         doesn't work with editable columns, and might be removed in the future.
 
     Examples
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/event_utils.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/event_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/map.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/markdown.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/markdown.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
         unsafe_allow_html : bool
             By default, any HTML tags found in the body will be escaped and
             therefore treated as pure text. This behavior may be turned off by
             setting this argument to True.
 
             That said, we *strongly advise against it*. It is hard to write
@@ -78,28 +80,28 @@
         Examples
         --------
         >>> import streamlit as st
         >>>
         >>> st.markdown("*Streamlit* is **really** ***cool***.")
         >>> st.markdown('''
         ...     :red[Streamlit] :orange[can] :green[write] :blue[text] :violet[in]
-        ...     :gray[pretty] :rainbow[colors].''')
+        ...     :gray[pretty] :rainbow[colors] and :blue-background[highlight] text.''')
         >>> st.markdown("Here's a bouquet &mdash;\
         ...             :tulip::cherry_blossom::rose::hibiscus::sunflower::blossom:")
         >>>
         >>> multi = '''If you end a line with two spaces,
         ... a soft return is used for the next line.
         ...
         ... Two (or more) newline characters in a row will result in a hard return.
         ... '''
         >>> st.markdown(multi)
 
         .. output::
            https://doc-markdown.streamlit.app/
-           height: 260px
+           height: 350px
 
         """
         markdown_proto = MarkdownProto()
 
         markdown_proto.body = clean_text(body)
         markdown_proto.allow_html = unsafe_allow_html
         markdown_proto.element_type = MarkdownProto.Type.NATIVE
@@ -173,16 +175,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
         unsafe_allow_html : bool
             By default, any HTML tags found in strings will be escaped and
             therefore treated as pure text. This behavior may be turned off by
             setting this argument to True.
 
             That said, *we strongly advise against it*. It is hard to write secure
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/media.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,18 +118,17 @@
               e.g. ``"2 minute"``, ``"20s"``, or ``"1m14s"``.
             * A ``timedelta`` object from `Python's built-in datetime library
               <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
               e.g. ``timedelta(seconds=70)``.
         loop: bool
             Whether the audio should loop playback.
         autoplay: bool
-            Whether the audio should start playing automatically.
-            Browsers will not autoplay audio files if the user has not interacted with
-            the page yet, for example by clicking on the page while it loads.
-            Defaults to False.
+            Whether the audio file should start playing automatically. This is
+            ``False`` by default. Browsers will not autoplay audio files if the
+            user has not interacted with the page by clicking somewhere.
 
         Examples
         --------
         To display an audio player for a local file, specify the file's string
         path and format.
 
         >>> import streamlit as st
@@ -223,15 +222,15 @@
             See https://tools.ietf.org/html/rfc4281 for more info.
 
         start_time: int, float, timedelta, str, or None
             The time from which the element should start playing. This can be
             one of the following:
 
             * ``None`` (default): The element plays from the beginning.
-            * An``int`` or ``float`` specifying the time in seconds. ``float``
+            * An ``int`` or ``float`` specifying the time in seconds. ``float``
               values are rounded down to whole seconds.
             * A string specifying the time in a format supported by `Pandas'
               Timedelta constructor <https://pandas.pydata.org/docs/reference/api/pandas.Timedelta.html>`_,
               e.g. ``"2 minute"``, ``"20s"``, or ``"1m14s"``.
             * A ``timedelta`` object from `Python's built-in datetime library
               <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
               e.g. ``timedelta(seconds=70)``.
@@ -271,22 +270,23 @@
               e.g. ``"2 minute"``, ``"20s"``, or ``"1m14s"``.
             * A ``timedelta`` object from `Python's built-in datetime library
               <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
               e.g. ``timedelta(seconds=70)``.
         loop: bool
             Whether the video should loop playback.
         autoplay: bool
-            Whether the video should start playing automatically.
-            Browsers will not autoplay video files if the user has not interacted with
-            the page yet, for example by clicking on the page while it loads.
-            To enable autoplay without user interaction, you can set muted=True.
-            Defaults to False.
+            Whether the video should start playing automatically. This is
+            ``False`` by default. Browsers will not autoplay unmuted videos
+            if the user has not interacted with the page by clicking somewhere.
+            To enable autoplay without user interaction, you must also set
+            ``muted=True``.
         muted: bool
-            Whether the video should play with the audio silenced. This can be used to
-            enable autoplay without user interaction. Defaults to False.
+            Whether the video should play with the audio silenced. This is
+            ``False`` by default. Use this in conjunction with ``autoplay=True``
+            to enable autoplay without user interaction.
 
         Example
         -------
         >>> import streamlit as st
         >>>
         >>> video_file = open('myvideo.mp4', 'rb')
         >>> video_bytes = video_file.read()
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/metric.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
         value : int, float, str, or None
              Value of the metric. None is rendered as a long dash.
         delta : int, float, str, or None
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/progress.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,16 +115,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
         Example
         -------
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/pyplot.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/snow.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/spinner.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/text.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/toast.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/toast.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,21 +65,35 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
-        icon : str or None
-            An optional argument that specifies an emoji to use as
-            the icon for the toast. Shortcodes are not allowed, please use a
-            single character instead. E.g. "🚨", "🔥", "🤖", etc.
-            Defaults to None, which means no icon is displayed.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
+
+        icon : str, None
+            An optional emoji or icon to display next to the alert. If ``icon``
+            is ``None`` (default), no icon is displayed. If ``icon`` is a
+            string, the following options are valid:
+
+            * A single-character emoji. For example, you can set ``icon="🚨"``
+              or ``icon="🔥"``. Emoji short codes are not supported.
+
+            * An icon from the Material Symbols library (outlined style) in the
+              format ``":material/icon_name:"`` where "icon_name" is the name
+              of the icon in snake case.
+
+              For example, ``icon=":material/thumb_up:"`` will display the
+              Thumb Up icon. Find additional icons in the `Material Symbols \
+              <https://fonts.google.com/icons?icon.set=Material+Symbols&icon.style=Outlined>`_
+              font library.
 
         Example
         -------
         >>> import streamlit as st
         >>>
         >>> st.toast('Your edited image was saved!', icon='😍')
         """
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/utils.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/button.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,16 +95,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
         key : str or int
             An optional string or integer to use as the unique key for the widget.
             If this is omitted, a key will be generated for the widget
@@ -136,18 +138,18 @@
             False otherwise.
 
         Example
         -------
         >>> import streamlit as st
         >>>
         >>> st.button("Reset", type="primary")
-        >>> if st.button('Say hello'):
-        ...     st.write('Why hello there')
+        >>> if st.button("Say hello"):
+        ...     st.write("Why hello there")
         ... else:
-        ...     st.write('Goodbye')
+        ...     st.write("Goodbye")
 
         .. output::
            https://doc-buton.streamlit.app/
            height: 220px
 
         """
         key = to_key(key)
@@ -215,16 +217,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents)
             render. Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
         data : str or bytes or file
             The contents of the file to be downloaded. See example below for
             caching techniques to avoid recomputing this data unnecessarily.
@@ -274,39 +278,39 @@
         Download a large DataFrame as a CSV:
 
         >>> import streamlit as st
         >>>
         >>> @st.cache_data
         ... def convert_df(df):
         ...     # IMPORTANT: Cache the conversion to prevent computation on every rerun
-        ...     return df.to_csv().encode('utf-8')
+        ...     return df.to_csv().encode("utf-8")
         >>>
         >>> csv = convert_df(my_large_df)
         >>>
         >>> st.download_button(
         ...     label="Download data as CSV",
         ...     data=csv,
-        ...     file_name='large_df.csv',
-        ...     mime='text/csv',
+        ...     file_name="large_df.csv",
+        ...     mime="text/csv",
         ... )
 
         Download a string as a file:
 
         >>> import streamlit as st
         >>>
         >>> text_contents = '''This is some text'''
-        >>> st.download_button('Download some text', text_contents)
+        >>> st.download_button("Download some text", text_contents)
 
         Download a binary file:
 
         >>> import streamlit as st
         >>>
-        >>> binary_contents = b'example content'
-        >>> # Defaults to 'application/octet-stream'
-        >>> st.download_button('Download binary file', binary_contents)
+        >>> binary_contents = b"example content"
+        >>> # Defaults to "application/octet-stream"
+        >>> st.download_button("Download binary file", binary_contents)
 
         Download an image:
 
         >>> import streamlit as st
         >>>
         >>> with open("flower.png", "rb") as file:
         ...     btn = st.download_button(
@@ -376,16 +380,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents)
             render. Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
         url : str
             The url to be opened on user click
         help : str
@@ -469,16 +475,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents)
             render. Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
         icon : str
             An optional argument that specifies an emoji to use as
             the icon for the link. Shortcodes are not allowed. Please use a
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/camera_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,16 +110,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,26 +136,43 @@
             The name of the message author. Can be "human"/"user" or
             "ai"/"assistant" to enable preset styling and avatars.
 
             Currently, the name is not shown in the UI but is only set as an
             accessibility label. For accessibility reasons, you should not use
             an empty string.
 
-        avatar : str, numpy.ndarray, or BytesIO
-            The avatar shown next to the message. Can be one of:
+        avatar : Anything supported by st.image, str, or None
+            The avatar shown next to the message.
 
-            * A single emoji, e.g. "🧑‍💻", "🤖", "🦖". Shortcodes are not supported.
+            If ``avatar`` is ``None`` (default), the icon will be determined
+            from ``name`` as follows:
 
-            * An image using one of the formats allowed for ``st.image``: path of a local
-                image file; URL to fetch the image from; an SVG image; array of shape
-                (w,h) or (w,h,1) for a monochrome image, (w,h,3) for a color image,
-                or (w,h,4) for an RGBA image.
+            * If ``name`` is ``"user"`` or ``"human"``, the message will have a
+              default user icon.
 
-            If None (default), uses default icons if ``name`` is "user",
-            "assistant", "ai", "human" or the first letter of the ``name`` value.
+            * If ``name`` is ``"ai"`` or ``"assistant"``, the message will have
+              a default bot icon.
+
+            * For all other values of ``name``, the message will show the first
+              letter of the name.
+
+            In addition to the types supported by ``st.image`` (like URLs or numpy
+            arrays), the following strings are valid:
+
+            * A single-character emoji. For example, you can set ``avatar="🧑‍💻"``
+              or ``avatar="🦖"``. Emoji short codes are not supported.
+
+            * An icon from the Material Symbols library (outlined style) in the
+              format ``":material/icon_name:"`` where "icon_name" is the name
+              of the icon in snake case.
+
+              For example, ``icon=":material/thumb_up:"`` will display the
+              Thumb Up icon. Find additional icons in the `Material Symbols \
+              <https://fonts.google.com/icons?icon.set=Material+Symbols&icon.style=Outlined>`_
+              font library.
 
         Returns
         -------
         Container
             A single container that can hold multiple elements.
 
         Examples
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/checkbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,16 +84,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -128,18 +130,18 @@
         bool
             Whether or not the checkbox is checked.
 
         Example
         -------
         >>> import streamlit as st
         >>>
-        >>> agree = st.checkbox('I agree')
+        >>> agree = st.checkbox("I agree")
         >>>
         >>> if agree:
-        ...     st.write('Great!')
+        ...     st.write("Great!")
 
         .. output::
            https://doc-checkbox.streamlit.app/
            height: 220px
 
         """
         ctx = get_script_run_ctx()
@@ -188,16 +190,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -232,18 +236,18 @@
         bool
             Whether or not the toggle is checked.
 
         Example
         -------
         >>> import streamlit as st
         >>>
-        >>> on = st.toggle('Activate feature')
+        >>> on = st.toggle("Activate feature")
         >>>
         >>> if on:
-        ...     st.write('Feature activated!')
+        ...     st.write("Feature activated!")
 
         .. output::
            https://doc-toggle.streamlit.app/
            height: 220px
 
         """
         ctx = get_script_run_ctx()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/color_picker.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -130,16 +132,16 @@
         str
             The selected color as a hex string.
 
         Example
         -------
         >>> import streamlit as st
         >>>
-        >>> color = st.color_picker('Pick A Color', '#00f900')
-        >>> st.write('The current color is', color)
+        >>> color = st.color_picker("Pick A Color", "#00f900")
+        >>> st.write("The current color is", color)
 
         .. output::
            https://doc-color-picker.streamlit.app/
            height: 335px
 
         """
         ctx = get_script_run_ctx()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/data_editor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/file_uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         kwargs: WidgetKwargs | None = None,
         *,  # keyword-only arguments:
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
     ) -> UploadedFile | list[UploadedFile] | None:
         r"""Display a file uploader widget.
         By default, uploaded files are limited to 200MB. You can configure
-        this using the `server.maxUploadSize` config option. For more info
+        this using the ``server.maxUploadSize`` config option. For more info
         on how to set config options, see
         https://docs.streamlit.io/library/advanced-features/configuration#set-configuration-options
 
         Parameters
         ----------
         label : str
             A short label explaining to the user what this file uploader is for.
@@ -262,16 +262,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/multiselect.py`

 * *Files 5% similar despite different names*

```diff
@@ -177,16 +177,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -236,19 +238,19 @@
             A list with the selected options
 
         Example
         -------
         >>> import streamlit as st
         >>>
         >>> options = st.multiselect(
-        ...     'What are your favorite colors',
-        ...     ['Green', 'Yellow', 'Red', 'Blue'],
-        ...     ['Yellow', 'Red'])
+        ...     "What are your favorite colors",
+        ...     ["Green", "Yellow", "Red", "Blue"],
+        ...     ["Yellow", "Red"])
         >>>
-        >>> st.write('You selected:', options)
+        >>> st.write("You selected:", options)
 
         .. output::
            https://doc-multiselect.streamlit.app/
            height: 420px
 
         """
         ctx = get_script_run_ctx()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/number_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,16 +154,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -218,27 +220,27 @@
             The current value of the numeric input widget or ``None`` if the widget
             is empty. The return type will match the data type of the value parameter.
 
         Example
         -------
         >>> import streamlit as st
         >>>
-        >>> number = st.number_input('Insert a number')
-        >>> st.write('The current number is ', number)
+        >>> number = st.number_input("Insert a number")
+        >>> st.write("The current number is ", number)
 
         .. output::
            https://doc-number-input.streamlit.app/
            height: 260px
 
         To initialize an empty number input, use ``None`` as the value:
 
         >>> import streamlit as st
         >>>
         >>> number = st.number_input("Insert a number", value=None, placeholder="Type a number...")
-        >>> st.write('The current number is ', number)
+        >>> st.write("The current number is ", number)
 
         .. output::
            https://doc-number-input-empty.streamlit.app/
            height: 260px
 
         """
         ctx = get_script_run_ctx()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/radio.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -185,18 +187,18 @@
         >>> import streamlit as st
         >>>
         >>> genre = st.radio(
         ...     "What's your favorite movie genre",
         ...     [":rainbow[Comedy]", "***Drama***", "Documentary :movie_camera:"],
         ...     captions = ["Laugh out loud.", "Get the popcorn.", "Never stop learning."])
         >>>
-        >>> if genre == ':rainbow[Comedy]':
-        ...     st.write('You selected comedy.')
+        >>> if genre == ":rainbow[Comedy]":
+        ...     st.write("You selected comedy.")
         ... else:
-        ...     st.write("You didn\'t select comedy.")
+        ...     st.write("You didn't select comedy.")
 
         .. output::
            https://doc-radio.streamlit.app/
            height: 300px
 
         To initialize an empty radio widget, use ``None`` as the index value:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/select_slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,16 +145,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -203,27 +205,27 @@
             the data type of the value parameter.
 
         Examples
         --------
         >>> import streamlit as st
         >>>
         >>> color = st.select_slider(
-        ...     'Select a color of the rainbow',
-        ...     options=['red', 'orange', 'yellow', 'green', 'blue', 'indigo', 'violet'])
-        >>> st.write('My favorite color is', color)
+        ...     "Select a color of the rainbow",
+        ...     options=["red", "orange", "yellow", "green", "blue", "indigo", "violet"])
+        >>> st.write("My favorite color is", color)
 
         And here's an example of a range select slider:
 
         >>> import streamlit as st
         >>>
         >>> start_color, end_color = st.select_slider(
-        ...     'Select a range of color wavelength',
-        ...     options=['red', 'orange', 'yellow', 'green', 'blue', 'indigo', 'violet'],
-        ...     value=('red', 'blue'))
-        >>> st.write('You selected wavelengths between', start_color, 'and', end_color)
+        ...     "Select a range of color wavelength",
+        ...     options=["red", "orange", "yellow", "green", "blue", "indigo", "violet"],
+        ...     value=("red", "blue"))
+        >>> st.write("You selected wavelengths between", start_color, "and", end_color)
 
         .. output::
            https://doc-select-slider.streamlit.app/
            height: 450px
 
         """
         ctx = get_script_run_ctx()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/selectbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,16 +109,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -146,15 +148,15 @@
             An optional callback invoked when this selectbox's value changes.
         args : tuple
             An optional tuple of args to pass to the callback.
         kwargs : dict
             An optional dict of kwargs to pass to the callback.
         placeholder : str
             A string to display when no options are selected.
-            Defaults to 'Choose an option'.
+            Defaults to "Choose an option".
         disabled : bool
             An optional boolean, which disables the selectbox if set to True.
             The default is False.
         label_visibility : "visible", "hidden", or "collapsed"
             The visibility of the label. If "hidden", the label doesn't show but there
             is still empty space for it above the widget (equivalent to label="").
             If "collapsed", both the label and the space are removed. Default is
@@ -166,18 +168,18 @@
             The selected option or ``None`` if no option is selected.
 
         Example
         -------
         >>> import streamlit as st
         >>>
         >>> option = st.selectbox(
-        ...     'How would you like to be contacted?',
-        ...     ('Email', 'Home phone', 'Mobile phone'))
+        ...     "How would you like to be contacted?",
+        ...     ("Email", "Home phone", "Mobile phone"))
         >>>
-        >>> st.write('You selected:', option)
+        >>> st.write("You selected:", option)
 
         .. output::
            https://doc-selectbox.streamlit.app/
            height: 320px
 
         To initialize an empty selectbox, use ``None`` as the index value:
 
@@ -186,15 +188,15 @@
         >>> option = st.selectbox(
         ...    "How would you like to be contacted?",
         ...    ("Email", "Home phone", "Mobile phone"),
         ...    index=None,
         ...    placeholder="Select contact method...",
         ... )
         >>>
-        >>> st.write('You selected:', option)
+        >>> st.write("You selected:", option)
 
         .. output::
            https://doc-selectbox-empty.streamlit.app/
            height: 320px
 
         """
         ctx = get_script_run_ctx()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,19 +187,19 @@
         #  can be annoying.
     ) -> Any:
         r"""Display a slider widget.
 
         This supports int, float, date, time, and datetime types.
 
         This also allows you to render a range slider by passing a two-element
-        tuple or list as the `value`.
+        tuple or list as the ``value``.
 
-        The difference between `st.slider` and `st.select_slider` is that
-        `slider` only accepts numerical or date/time data and takes a range as
-        input, while `select_slider` accepts any datatype and takes an iterable
+        The difference between ``st.slider`` and ``st.select_slider`` is that
+        ``slider`` only accepts numerical or date/time data and takes a range as
+        input, while ``select_slider`` accepts any datatype and takes an iterable
         set of options.
 
         .. note::
             Integer values exceeding +/- ``(1<<53) - 1`` cannot be accurately
             stored or returned by the widget due to serialization contstraints
             between the Python server and JavaScript client. You must handle
             such numbers as floats, leading to a loss in precision.
@@ -219,16 +219,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -287,25 +289,25 @@
             The current value of the slider widget. The return type will match
             the data type of the value parameter.
 
         Examples
         --------
         >>> import streamlit as st
         >>>
-        >>> age = st.slider('How old are you?', 0, 130, 25)
-        >>> st.write("I'm ", age, 'years old')
+        >>> age = st.slider("How old are you?", 0, 130, 25)
+        >>> st.write("I'm ", age, "years old")
 
         And here's an example of a range slider:
 
         >>> import streamlit as st
         >>>
         >>> values = st.slider(
-        ...     'Select a range of values',
+        ...     "Select a range of values",
         ...     0.0, 100.0, (25.0, 75.0))
-        >>> st.write('Values:', values)
+        >>> st.write("Values:", values)
 
         This is a range time slider:
 
         >>> import streamlit as st
         >>> from datetime import time
         >>>
         >>> appointment = st.slider(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/text_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,16 +148,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -208,16 +210,16 @@
             The current value of the text input widget or ``None`` if no value has been
             provided by the user.
 
         Example
         -------
         >>> import streamlit as st
         >>>
-        >>> title = st.text_input('Movie title', 'Life of Brian')
-        >>> st.write('The current movie title is', title)
+        >>> title = st.text_input("Movie title", "Life of Brian")
+        >>> st.write("The current movie title is", title)
 
         .. output::
            https://doc-text-input.streamlit.app/
            height: 260px
 
         """
         ctx = get_script_run_ctx()
@@ -414,16 +416,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -477,15 +481,15 @@
         ...     "It was the best of times, it was the worst of times, it was the age of "
         ...     "wisdom, it was the age of foolishness, it was the epoch of belief, it "
         ...     "was the epoch of incredulity, it was the season of Light, it was the "
         ...     "season of Darkness, it was the spring of hope, it was the winter of "
         ...     "despair, (...)",
         ...     )
         >>>
-        >>> st.write(f'You wrote {len(txt)} characters.')
+        >>> st.write(f"You wrote {len(txt)} characters.")
 
         .. output::
            https://doc-text-area.streamlit.app/
            height: 300px
 
         """
         ctx = get_script_run_ctx()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/widgets/time_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,16 +319,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -370,28 +372,28 @@
             selected.
 
         Example
         -------
         >>> import datetime
         >>> import streamlit as st
         >>>
-        >>> t = st.time_input('Set an alarm for', datetime.time(8, 45))
-        >>> st.write('Alarm is set for', t)
+        >>> t = st.time_input("Set an alarm for", datetime.time(8, 45))
+        >>> st.write("Alarm is set for", t)
 
         .. output::
            https://doc-time-input.streamlit.app/
            height: 260px
 
         To initialize an empty time input, use ``None`` as the value:
 
         >>> import datetime
         >>> import streamlit as st
         >>>
-        >>> t = st.time_input('Set an alarm for', value=None)
-        >>> st.write('Alarm is set for', t)
+        >>> t = st.time_input("Set an alarm for", value=None)
+        >>> st.write("Alarm is set for", t)
 
         .. output::
            https://doc-time-input-empty.streamlit.app/
            height: 260px
 
         """
         ctx = get_script_run_ctx()
@@ -544,16 +546,18 @@
 
             * LaTeX expressions, by wrapping them in "$" or "$$" (the "$$"
               must be on their own lines). Supported LaTeX functions are listed
               at https://katex.org/docs/supported.html.
 
             * Colored text and background colors for text, using the syntax
               ``:color[text to be colored]`` and ``:color-background[text to be colored]``,
-              respectively — where ``color`` needs to be replaced with any of the following
+              respectively. ``color`` must be replaced with any of the following
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
+              For example, you can use ``:orange[your text here]`` or
+              ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents) render.
             Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
 
             For accessibility reasons, you should never set an empty label (label="")
             but hide it with label_visibility if needed. In the future, we may disallow
@@ -581,15 +585,15 @@
             An optional callback invoked when this date_input's value changes.
         args : tuple
             An optional tuple of args to pass to the callback.
         kwargs : dict
             An optional dict of kwargs to pass to the callback.
         format : str
             A format string controlling how the interface should display dates.
-            Supports “YYYY/MM/DD” (default), “DD/MM/YYYY”, or “MM/DD/YYYY”.
+            Supports "YYYY/MM/DD" (default), "DD/MM/YYYY", or "MM/DD/YYYY".
             You may also use a period (.) or hyphen (-) as separators.
         disabled : bool
             An optional boolean, which disables the date input if set to True.
             The default is False.
         label_visibility : "visible", "hidden", or "collapsed"
             The visibility of the label. If "hidden", the label doesn't show but there
             is still empty space for it above the widget (equivalent to label="").
@@ -605,15 +609,15 @@
 
         Examples
         --------
         >>> import datetime
         >>> import streamlit as st
         >>>
         >>> d = st.date_input("When's your birthday", datetime.date(2019, 7, 6))
-        >>> st.write('Your birthday is:', d)
+        >>> st.write("Your birthday is:", d)
 
         .. output::
            https://doc-date-input.streamlit.app/
            height: 380px
 
         >>> import datetime
         >>> import streamlit as st
@@ -638,15 +642,15 @@
 
         To initialize an empty date input, use ``None`` as the value:
 
         >>> import datetime
         >>> import streamlit as st
         >>>
         >>> d = st.date_input("When's your birthday", value=None)
-        >>> st.write('Your birthday is:', d)
+        >>> st.write("Your birthday is:", d)
 
         .. output::
            https://doc-date-input-empty.streamlit.app/
            height: 380px
 
         """
         ctx = get_script_run_ctx()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/elements/write.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/emojis.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/env_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/error_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/errors.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/external/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/file_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/folder_black_list.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/git_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/hello/Hello.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/hello/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/hello/utils.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/js_number.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/logger.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/material_icon_names.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/material_icon_names.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/net_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/platform.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Toast_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240501/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/app_session.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cache_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,17 +300,48 @@
                         so `st.cache_data` can serialize and cache it."""
                     )
                 raise UnserializableReturnValueError(
                     return_value=computed_value, func=self._info.func
                 )
 
     def clear(self, *args, **kwargs):
-        """Clear the wrapped function's associated cache.
-        If no arguments are passed, clear the cache of all values.
-        If args/kwargs are provided, clear the cached value for these arguments only."""
+        """Clear the cached function's associated cache.
+
+        If no arguments are passed, Streamlit will clear all values cached for
+        the function. If arguments are passed, Streamlit will clear the cached
+        value for these arguments only.
+
+        Parameters
+        ----------
+        *args: Any
+            Arguments of the cached functions.
+        **kwargs: Any
+            Keyword arguments of the cached function.
+
+        Example
+        -------
+        >>> import streamlit as st
+        >>> import time
+        >>>
+        >>> @st.cache_data
+        >>> def foo(bar):
+        >>>     time.sleep(2)
+        >>>     st.write(f"Executed foo({bar}).")
+        >>>     return bar
+        >>>
+        >>> if st.button("Clear all cached values for `foo`", on_click=foo.clear):
+        >>>     foo.clear()
+        >>>
+        >>> if st.button("Clear the cached value of `foo(1)`"):
+        >>>     foo.clear(1)
+        >>>
+        >>> foo(1)
+        >>> foo(2)
+
+        """
         cache = self._info.get_function_cache(self._function_key)
         if args or kwargs:
             key = _make_value_key(
                 cache_type=self._info.cache_type,
                 func=self._info.func,
                 func_args=args,
                 func_kwargs=kwargs,
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/credentials.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/fragment.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/fragment.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/legacy_caching/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/legacy_caching/caching.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/legacy_caching/hashing.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/runtime.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/script_data.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/secrets.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/common.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/query_params_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -167,30 +167,40 @@
         ...
 
     @overload
     def from_dict(self, mapping: SupportsKeysAndGetItem[str, str]) -> None:
         ...
 
     @gather_metrics("query_params.from_dict")
-    def from_dict(self, other):
+    def from_dict(self, params):
         """
         Set all of the query parameters from a dictionary or dictionary-like object.
 
-        This method primarily exists for advanced users who want to be able to control
-        multiple query string parameters in a single update. To set individual
-        query string parameters you should still use `st.query_params["parameter"] = "value"`
-        or `st.query_params.parameter = "value"`.
-
-        `embed` and `embed_options` may not be set via this method and may not be keys in the
-        `other` dictionary.
-
-        Note that this method is NOT a direct inverse of `st.query_params.to_dict()` when
-        the URL query string contains multiple values for a single key. A true inverse
-        operation for from_dict is `{key: st.query_params.get_all(key) for key st.query_params}`.
+        This method primarily exists for advanced users who want to control
+        multiple query parameters in a single update. To set individual query
+        parameters, use key or attribute notation instead.
+
+        This method inherits limitations from ``st.query_params`` and can't be
+        used to set embedding options as described in `Embed your app \
+        <https://docs.streamlit.io/deploy/streamlit-community-cloud/share-your-app/embed-your-app#embed-options>`_.
+
+        To handle repeated keys, the value in a key-value pair should be a list.
+
+        .. note::
+            ``.from_dict()`` is not a direct inverse of ``.to_dict()`` if
+            you are working with repeated keys. A true inverse operation is
+            ``{key: st.query_params.get_all(key) for key st.query_params}``.
 
         Parameters
+        ----------
+        params: dict
+            A dictionary used to replace the current query parameters.
+
+        Example
         -------
-        other: SupportsKeysAndGetItem[str, str] | Iterable[tuple[str, str]]
-            A dictionary used to replace the current query_params.
+        >>> import streamlit as st
+        >>>
+        >>> st.query_params.from_dict({"foo": "bar", "baz": [1, "two"]})
+
         """
         with get_session_state().query_params() as qp:
-            return qp.from_dict(other)
+            return qp.from_dict(params)
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/stats.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/source_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/favicon.png` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/index.html` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/css/3092.95a45cfe.chunk.css` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/css/3092.95a45cfe.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/css/3466.8b8f33d6.chunk.css` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/css/3466.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/css/43.e3b876c5.chunk.css` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/css/43.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/css/main.3aaaea00.css` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/css/main.3aaaea00.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1168.fc5c673b.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1168.fc5c673b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1307.8ea033f1.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1307.8ea033f1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/178.7bea8c5d.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/178.7bea8c5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/1792.b8efa879.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/1792.b8efa879.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2469.3e9c3ce9.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2469.3e9c3ce9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2736.914069e5.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2736.914069e5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3061.67758376.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3061.67758376.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3092.bc07c48b.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3092.bc07c48b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3466.05d62820.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3466.05d62820.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3513.e3e7300a.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3513.e3e7300a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/3631.be5c35fa.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/3631.be5c35fa.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4113.1e7eff4d.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4113.1e7eff4d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4253.749d5244.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4253.749d5244.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/43.c6749504.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/43.c6749504.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4319.bf1c86bf.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4319.bf1c86bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4477.e10e4373.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4477.e10e4373.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/4666.c4b22a63.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/4666.c4b22a63.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/474.87506447.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/474.87506447.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5345.65c91ee7.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5345.65c91ee7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6013.64cd6d28.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6013.64cd6d28.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6150.427a30f5.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6150.427a30f5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/656.7150a933.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/656.7150a933.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/6853.3cbd385e.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/6853.3cbd385e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7217.d970c074.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7217.d970c074.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7323.2808d029.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7323.2808d029.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7602.e8abc06b.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7602.e8abc06b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/7805.51638fbc.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/7805.51638fbc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8427.65ddaf36.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8427.65ddaf36.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8477.7419a0aa.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8477.7419a0aa.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8492.3e609489.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8492.3e609489.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8536.f13dff49.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8536.f13dff49.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9330.2b4c99e0.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9330.2b4c99e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9336.2d95d840.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9336.2d95d840.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9758.6e6d8662.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9758.6e6d8662.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/main.af77b7ba.js` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/main.af77b7ba.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/js/main.af77b7ba.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/js/main.af77b7ba.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.33.1.dev20240501/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/string_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/temporary_directory.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/testing/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/testing/v1/util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/time_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/type_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/url_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/user_info.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/version.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/watcher/util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/bootstrap.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/cli.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/__init__.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/routes.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/server.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/server_util.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.33.1.dev20240501/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.33.1.dev20240430
+Version: 1.33.1.dev20240501
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.33.1.dev20240430/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.33.1.dev20240501/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240430/tests/testutil.py` & `streamlit_nightly-1.33.1.dev20240501/tests/testutil.py`

 * *Files identical despite different names*

